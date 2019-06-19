1. Why is Lettuce the default Redis client used in Spring Session Redis?

片段：Jedis is a straight-forward Redis client that is not thread-safe when applications want to share a single Jedis instance across multiple threads. The approach to use Jedis in a multi-threaded environment is to use connection pooling. Each concurrent thread using Jedis gets its own Jedis instance for the duration of Jedis interaction. Connection pooling comes at the cost of a physical connection per Jedis instance which increases the number of Redis connections.

Lettuce is built on netty and connection instances (StatefulRedisConnection) can be shared across multiple threads. So a multi-threaded application can use a single connection
regardless the number of concurrent threads that interact with Lettuce.

Limiting the number of connections can be required when using connection limits on Redis or when the number of connections grows beyond a reasonable connection count.

Does this make sense?

来源：https://github.com/spring-projects/spring-session/issues/789
