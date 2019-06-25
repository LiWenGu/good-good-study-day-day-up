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
