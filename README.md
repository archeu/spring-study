# study-notes

图解学习笔记，大图少字。在线阅读：https://archeu.github.io/study-notes/

每个主题一个目录，首页 `index.html` 按主题分组列出所有页面。

## Spring

| # | 页面 | 内容 |
|---|------|------|
| 01 | [Spring MVC 请求关卡](https://archeu.github.io/study-notes/spring/spring-web-gates.html) | Filter、Interceptor、WebMvcConfigurer 的区别、生命周期和用途 |
| 02 | [Spring AOP 与事务](https://archeu.github.io/study-notes/spring/spring-aop-tx.html) | 代理、切面、通知，@Transactional 的提交回滚、传播、隔离和失效场景 |
| 03 | [Spring Boot 自动配置](https://archeu.github.io/study-notes/spring/spring-boot-autoconfig.html) | starter、自动配置清单、条件注解，启动时序和自定义 starter |
| 04 | [Bean 生命周期与循环依赖](https://archeu.github.io/study-notes/spring/spring-bean-lifecycle.html) | 十四站生命周期、回调顺序、作用域，三级缓存怎么解循环依赖 |
| 05 | [Spring Security 认证与授权](https://archeu.github.io/study-notes/spring/spring-security.html) | 过滤器链、核验台、工牌和门禁，401 和 403 从哪来，Security 5 和 6 的写法差别 |
| 06 | [Spring MVC 请求处理流程](https://archeu.github.io/study-notes/spring/spring-mvc-flow.html) | DispatcherServlet 的 doDispatch 八步，参数解析、页面和 JSON 两种返回、异常善后 |
| 07 | [Spring Boot 启动流程](https://archeu.github.io/study-notes/spring/spring-boot-startup.html) | run() 的四段路、refresh 十二步、Tomcat 什么时候开端口，事件顺序、扩展点和启动失败 |
| 08 | [Spring 事件机制](https://archeu.github.io/study-notes/spring/spring-events.html) | 发布者、广播站、监听器，同步、@Async、@TransactionalEventListener 怎么选，事件实验台 |
| 09 | [Spring IoC 与依赖注入](https://archeu.github.io/study-notes/spring/spring-ioc-di.html) | 容器里有什么、图纸从哪来、三种注入写法，同类型多个 Bean 时怎么选的注入裁判 |
| 10 | [Spring AOP 代理原理](https://archeu.github.io/study-notes/spring/spring-aop-proxy.html) | 替身什么时候换上、JDK 代理和 CGLIB、调用怎样穿过拦截器链，替身管不到的地方 |
| 11 | [Spring @Async 与线程池](https://archeu.github.io/study-notes/spring/spring-async-pool.html) | @Async 背后的派单员、用哪个线程池、四步规则和拒绝策略，线程池模拟器 |

## MyBatis

| # | 页面 | 内容 |
|---|------|------|
| 01 | [MyBatis 执行流程](https://archeu.github.io/study-notes/mybatis/mybatis-flow.html) | 启动时编好 SQL 手册，一次调用经过 MapperProxy、SqlSession、Executor 和 JDBC，两级缓存、#{} 与 ${}、插件 |
| 02 | [MyBatis 与 Spring 事务](https://archeu.github.io/study-notes/mybatis/mybatis-spring-tx.html) | 同一个 DataSource、线程上的储物柜、SqlSessionTemplate 复用会话，谁来提交，五个剧情看回滚和坑 |
| 03 | [MyBatis 插件与分页](https://archeu.github.io/study-notes/mybatis/mybatis-plugin-page.html) | 四个能拦的对象、Plugin.wrap 套娃和登记顺序，PageHelper 和 MyBatis-Plus 怎么分页，深分页 |
| 04 | [MyBatis 缓存与 Caffeine](https://archeu.github.io/study-notes/mybatis/mybatis-cache.html) | 一级、二级缓存怎么存怎么清，五个剧情看旧数据，和 Caffeine 逐项对比，LRU 与 W-TinyLFU 命中率 |
| 05 | [MyBatis-Plus 原理](https://archeu.github.io/study-notes/mybatis/mybatis-plus.html) | 启动时注入 SQL、Wrapper 怎么变成 SQL、自动填充和雪花 ID、插件总管和顺序，saveBatch 怎么批量 |

## 数据库

| # | 页面 | 内容 |
|---|------|------|
| 01 | [连接池与事务性能](https://archeu.github.io/study-notes/database/db-pool-tx-perf.html) | 为什么建连接贵、池子开多大、事务怎么吃掉连接、提交落盘和长事务、驱动参数，连接池模拟器 |
| 02 | [MySQL MVCC 与锁](https://archeu.github.io/study-notes/database/mysql-mvcc-lock.html) | 隐藏列和版本链、Read View 怎么判断看得见、快照读和当前读、四种行锁和死锁，MVCC 实验台和锁地图 |

## 性能

| # | 页面 | 内容 |
|---|------|------|
| 01 | [系统压测](https://archeu.github.io/study-notes/perf/load-testing.html) | 看哪五个数、六种压测、吞吐为什么会到顶、八类常见瓶颈的原理和解法、方案优劣和工具对比，压测曲线和瓶颈实验台 |

## Redis

| # | 页面 | 内容 |
|---|------|------|
| 01 | [缓存穿透、击穿与雪崩](https://archeu.github.io/study-notes/redis/cache-problems.html) | 三种漏法怎么发生、布隆过滤器、互斥锁和逻辑过期、过期时间打散和高可用，十种防护的代价，数据库压力实验台 |
| 02 | [Redis 持久化 RDB 与 AOF](https://archeu.github.io/study-notes/redis/redis-persistence.html) | 拍照和记账、fork 与写时复制、三种刷盘策略、AOF 重写、混合持久化和多文件 AOF，宕机实验台 |
| 03 | [Redis 主从、哨兵与集群](https://archeu.github.io/study-notes/redis/redis-ha-cluster.html) | 全量和部分同步、哨兵怎么判死和换主、16384 个槽和 hash tag，故障转移演示和槽位计算器 |
| 04 | [Redis 数据结构与编码](https://archeu.github.io/study-notes/redis/redis-data-encoding.html) | 五种类型和八种编码、SDS 与 embstr、listpack 与 quicklist、渐进式 rehash、跳表，编码观察器 |
| 05 | [Redis 过期删除与内存淘汰](https://archeu.github.io/study-notes/redis/redis-eviction-expire.html) | 惰性删除加定期巡逻、八种淘汰策略、近似 LRU 的抽样和候选池、LFU 计数器，巡逻实验台和淘汰准确度对比 |
| 06 | [Redis 分布式锁](https://archeu.github.io/study-notes/redis/redis-distributed-lock.html) | 五次进化、令牌和 Lua 解锁、Redisson 看门狗，锁与事务的顺序、主从切换丢锁、RedLock 和 fencing token，事故实验台 |
| 07 | [Redis 线程模型与 IO 多路复用](https://archeu.github.io/study-notes/redis/redis-threading-io.html) | 单线程为什么快、select/poll/epoll、事件循环演示、慢命令怎么堵住所有人、I/O 线程和 Pipeline |
| 08 | [Redis 大 key 与热 key](https://archeu.github.io/study-notes/redis/redis-bigkey-hotkey.html) | 多大算大、危害和拆分，热 key 为什么加机器没用、本地缓存和复制打散，怎么发现，大 key 计算器和热 key 实验台 |
| 09 | [Redis Stream 与消息队列](https://archeu.github.io/study-notes/redis/redis-stream-mq.html) | List、Pub/Sub、Stream 三代对比，消费组、PEL、ACK 和认领，至少一次与幂等，延迟消息，消费组实验台 |
| 10 | [Redis Lua 脚本与事务](https://archeu.github.io/study-notes/redis/redis-lua-tx.html) | MULTI/EXEC/WATCH、出错为什么不回滚、Lua 的写法和 EVALSHA、Redis 7 Functions，最后一件库存两人抢 |
| 11 | [布隆过滤器与 HyperLogLog](https://archeu.github.io/study-notes/redis/redis-bloom-hll.html) | 位数组和 k 个哈希、误判率实验室、容量怎么算、抛硬币估人数、16384 个桶，UV 统计和选型 |

## Kafka

| # | 页面 | 内容 |
|---|------|------|
| 01 | [Kafka 消息可靠性与消费组](https://archeu.github.io/study-notes/kafka/kafka-reliability-group.html) | 六步学习法：acks 和 ISR、min.insync.replicas、offset 提交时机、消费组和 rebalance、幂等与死信，故障实验台和消费组实验台（关键行为本机集群实测） |
| 02 | [Kafka 存储：segment、索引、页缓存与零拷贝](https://archeu.github.io/study-notes/kafka/kafka-storage-zerocopy.html) | 分段和稀疏索引怎么查、页缓存为什么比 JVM 缓存好、sendfile 少了哪几次拷贝、retention 为什么不准、回放拖慢实时和 TLS 的代价，查找、零拷贝、页缓存三个实验台 |
