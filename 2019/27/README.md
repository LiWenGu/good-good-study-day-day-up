# 07.02

## Java魔法类：Unsafe应用解析

>![](https://p1.meituan.net/travelcube/f182555953e29cec76497ebaec526fd1297846.png)

来源：https://tech.meituan.com/2019/02/14/talk-about-java-magic-class-unsafe.html

# 07.03

## 寻找一种易于理解的一致性算法（扩展版）

>Raft 是一种为了管理复制日志的一致性算法。它提供了和 Paxos 算法相同的功能和性能，但是它的算法结构和 Paxos 不同，使得 Raft 算法更加容易理解并且更容易构建实际的系统。为了提升可理解性，Raft 将一致性算法分解成了几个关键模块，例如领导人选举、日志复制和安全性。同时它通过实施一个更强的一致性来减少需要考虑的状态的数量。从一个用户研究的结果可以证明，对于学生而言，Raft 算法比 Paxos 算法更加容易学习。Raft 算法还包括一个新的机制来允许集群成员的动态改变，它利用重叠的大多数来保证安全性。

来源：  
https://github.com/maemual/raft-zh_cn/blob/master/raft-zh_cn.md  
http://thinkinjava.cn/2018/10/26/2018/2018-10-26-Raft%20%E7%AE%97%E6%B3%95%E6%B5%93%E7%BC%A9/

# 07.04

## 从一次 Snowflake 异常说起

>大家应该都知道雪花算法存在的缺点是：  
>1. 依赖机器时钟，如果机器时钟回拨，会导致重复ID生成  
>2. 在单机上是递增的，但是由于设计到分布式环境，每台机器上的时钟不可能完全同步，有时候会出现不是全局递增的情况（此缺点可以认为无所谓，一般分布式ID只要求趋势递增，并不会严格要求递增～90%的需求都只要求趋势递增）

来源：https://blog.csdn.net/X5fnncxzq4/article/details/79549514
