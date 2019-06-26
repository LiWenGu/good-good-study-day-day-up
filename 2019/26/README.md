# 06.24

## System.exit和Runtime.halt区别

>现在runtime的halt比较好理解了，他不会执行钩子函数和finalizer方法，而是直接退出。

来源：https://www.cnblogs.com/yanbit/p/4739473.html

## Apache Tomcat 相关漏洞

>By not sending WINDOW_UPDATE messages for the connection window (stream 0) clients were able to cause server-side threads to block eventually leading to thread exhaustion and a DoS  
>The issue was made public on 20 June 2019.  
>Affects: 8.5.0 to 8.5.40

来源：https://tomcat.apache.org/security-8.html

# 06.25

## Springboot 2.0选择HikariCP作为默认数据库连接池的五大理由

>![](https://github.com/brettwooldridge/HikariCP/wiki/HikariCP-bench-2.6.0.png)

来源：http://blog.didispace.com/Springboot-2-0-HikariCP-default-reason/

# 06.26

## Spring计时器StopWatch的使用

>Spring提供的计时器StopWatch对于秒、毫秒为单位方便计时的程序，尤其是单线程、顺序执行程序的时间特性的统计输出支持比较好

来源：https://blog.csdn.net/ioe_gaoyong/article/details/22788789

## Guava官方文档-RateLimiter类

>RateLimiter使用的是一种叫令牌桶的流控算法，RateLimiter会按照一定的频率往桶里扔令牌，线程拿到令牌才能执行，比如你希望自己的应用程序QPS不要超过1000，那么RateLimiter设置1000的速率后，就会每秒往桶里扔1000个令牌。

来源：http://ifeve.com/guava-ratelimiter/
