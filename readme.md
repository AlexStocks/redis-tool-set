# Redis tool list #

Here is a Redis tool list. I hope you will find one or two of them that you'd like to try out.


Table of Contents
=================
  * [Cloud Native](#cloud-native)
  * [Redis Cluster](#redis-cluster)
  * [Redis Variety](#redis-variety)
  * [Redis Proxy](#redis-proxy)
  * [Redis Module](#redis-module)
  * [Redis Client](#redis-client)
  * [Redis Data Migration](#redis-data-migration)
  * [Redis Monitor](#redis-monitor)
  * [Redis Admin Web &amp; UI](#redis-admin-web--ui)
  * [Redis Golang Packages](#redis-golang-packages)
  * [Redis Based Lock&amp;Cache](#redis-based-lockcache)
  * [Redis Ecosystem](#redis-ecosystem)

---
## Cloud Native

| Project Name | Stars | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [redis-operator](https://github.com/OT-CONTAINER-KIT/redis-operator) | 508(2023/07/13) | Go | About
A golang based redis operator that will make/oversee Redis standalone/cluster/replication/sentinel mode setup on top of the Kubernetes. |

---
## Redis Cluster

| Project Name | Stars | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [Codis](https://github.com/CodisLabs/codis) | 9113(2019/04/06) | Go | Codis is a proxy based high performance Redis cluster solution written in Go. It is production-ready and widely used at wandoujia.com and many companies. |
| [x-pipe](https://github.com/ctripcorp/x-pipe) | 791 | Java | Redis 多数据中心集群，一是为了提升可用性，解决数据中心 DR(Disaster Recovery) 问题，二是提升访问性能，每个数据中心可以读取当前数据中心的数据，无需跨机房读数据。|
| [cc](https://github.com/ksarch-saas/cc) | 32(2019/04/06) | Go & Js | This is a Redis Cluster Controller to control the state of the cluster nodes and provide http api and tools(both command line and web ui). Star: 17(until 2017/08/19). |
| [godis](https://github.com/HDT3213/godis) | 629 | Go | Godis is a golang implementation of Redis Server, which intents to provide an example of writing a high concurrent middleware using golang. |

---
## Redis Variety

| Project Name | Stars(until 2019/04/14) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [Pika](https://github.com/Qihoo360/pika) | 2679 | C++ | Pika is a nosql compatible with redis protocol, it is developed by Qihoo's DBA and infrastructure team, and it is widely used in QiHoo. Pika is a persistent huge storage service , compatible with the vast majority of redis interfaces (details), including string, hash, list, zset, set and management interfaces. With the huge amount of data stored, redis may suffer for a capacity bottleneck, and pika was born for solving it. Except huge storage capacity, pika also support master-slave mode by slaveof command, including full and partial synchronization. |
| [webdis](https://github.com/nicolasff/webdis) | 2099 | C | A very simple web server providing an HTTP interface to Redis. It uses hiredis, jansson, libevent, and [http-parser](https://github.com/nodejs/http-parser) |
| [ardb](https://github.com/yinqiwen/ardb) | 1309 | C++ | A redis protocol compatible nosql, it support multiple storage engines as backend like Google's LevelDB, Facebook's RocksDB, OpenLDAP's LMDB, PerconaFT, WiredTiger, ForestDB. |
| [Pedis](https://github.com/fastio/pedis) | 1027 | C++ | NoSQL data store using the SEASTAR framework, compatible with REDIS. |
| [Qedis](https://github.com/loveyacper/Qedis) | 54 | C++ | A C++11 implementation of distributed redis server, use Leveldb for persist storage.(including cluster) |
| [AliRedis](http://blog.sina.com.cn/s/blog_e59371cc0101br74.html) | | C | AliRedis, which is developed by Alibaba， use a new nginx-like(one-master-multi-worker) framework, in order to get full use of the CPU cores. |
| [Pushlet](https://github.com/wjw465150/Pushlet/tree/branch-redis) | 139 | JavaScript | Pushlet 是一个开源的 Comet 框架,Pushlet使用了观察者模型：客户端发送请求，订阅感兴趣的事件；服务器端为每个客户端分配一个会话 ID 作为标记，事件源会把新产生的事件以多播的方式发送到订阅者的事件队列里。 |
| [xredis-server](https://github.com/0xsky/xredis-server) | 50 | C++ | redis-server is a redis server framework library write by C++, using this library you can develop redis protocol compatible server easily. xredis-server requires libevent. |
| [qdb](https://github.com/reborndb/qdb) | 327 | Go | A fast, high availability, fully Redis compatible store engine. |
| [vire](https://github.com/vipshop/vire) | 167 | C | vire (pronounced "vip-redis") is a multithread redis(based on redis-3.2.0) maintains in vipshop. |
| [swapdb](https://github.com/JingchengLi/swapdb) | 269 | C | A redis compatiable storage which support data exchange between memory and disk. |
| [ApsaraCache](https://github.com/alibaba/ApsaraCache) | 848 | C |ApsaraCache is based on the Redis official release 4.0 and has many features and performance enhancements. ApsaraCache has proven to be very stable and efficient in production environment. |
| [titan](https://github.com/distributedio/titan) | 658 | Go | A distributed implementation of Redis compatible layer based on [TiKV](https://github.com/tikv/tikv/). |
| [KeyDB](https://github.com/JohnSully/KeyDB) | 1459 | C++ | a high performance fork of Redis focussing on multithreading, memory efficiency, and high throughput. In addition to multithreading KeyDB also has features only available in Redis Enterprise such as FLASH storage support, and some not available at all such as direct backup to AWS S3. |
| [rsedis](https://github.com/seppo0010/rsedis) | 1218 | Rust | Redis re-implemented in Rust |
| [redis-windows](https://github.com/ServiceStack/redis-windows) | 2400 | C | Vagrant redis configuration and the binary releases of MS Open Tech redis port of windows |
| [Tendis](https://github.com/tencent/Tendis) | 717 | C | a high-performance distributed storage system fully compatible with the Redis protocol. Using RocksDB as storage engine. All data is stored in RocksDB in a specific format, supporting PB-level storage capacity. |
| [dragonfly](https://github.com/dragonflydb/dragonfly) | 18900 | C++ | An in-memory data store built for modern application workloads. Fully compatible with Redis and Memcached APIs, Dragonfly requires no code changes to adopt. Compared to legacy in-memory datastores, Dragonfly delivers 25X more throughput, higher cache hit rates with lower tail latency, and effortless vertical scalability. |
| [rsedis](https://github.com/seppo0010/rsedis) | 1700 | Rust | Redis re-implemented in Rust | 

---
## Redis Proxy

| Project Name | Stars(until 2019/04/14) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [aster](https://github.com/wayslog/aster) | 41 | Rust | Aster is a light, fast and powerful cache proxy written in rust. the same with twemproxy but support multi-threads.  Make redis cluster can be used to simple redis client.  |
| [undermoon](https://github.com/doyoubi/undermoon) | 63 | Rust | Aims to provide a Redis cluster solution based on Redis Cluster Protocol supporting multiple tenants and easy scaling. |
| [twemproxy](https://github.com/twitter/twemproxy) | 8920 | C | twemproxy (pronounced "two-em-proxy"), aka nutcracker is a fast and lightweight proxy for [memcached](http://www.memcached.org/) and [redis](http://redis.io/) protocol. It was built primarily to reduce the number of connections to the caching servers on the backend. This, together with protocol pipelining and sharding enables you to horizontally scale your distributed caching architecture.|
| [redis-cerberus](https://github.com/projecteru/redis-cerberus) | 305 | C++ | redis-cerberus是一个Redis集群代理程序，早期是为了在使用Redis集群的同时兼容旧客户端和应用程序库而开发的。后续开发过程中加入了基于Redis集群主从模式的读写分离特性。|
| [Redsmin proxy deamon](https://github.com/Redsmin/proxy) | 78 | JavaScript | Access local redis instance from Redsmin https://redsmin.com. Redsmin and Redsmin proxy communicate through a secure connection using the TLS 1.2 protocol so no one will be able to inspect the data looking at the traffic.  |
| [bilitw](https://github.com/anewhuahua/bilitw) | 57 | C | bilitw (bilibili twemproxy), which introduce multi process of twemproxy(one master and mutli worker), is order to get full use of the CPU cores. |
| [Corvus](https://github.com/eleme/corvus) | 640 | C | A fast and lightweight Redis Cluster Proxy for Redis 3.0.  |
| [twemproxy-163](https://github.com/helifu/twemproxy-163) | 34 | C | twemproxy-163 supports redis-server failover by communicating with redis-sentinel. |
| [twemproxies](https://github.com/vipshop/twemproxies) | 67 | C | twemproxies ( nutcrackers ) is a multithread, fast and lightweight proxy for memcached and redis protocol. It was built primarily to reduce the number of connections to the caching servers on the backend. This, together with protocol pipelining and sharding enables you to horizontally scale your distributed caching architecture. |
| [twemproxy-vip](https://github.com/vipshop/twemproxy-vip) | 43 | C | twemproxy maintained and used at vipshop.  |
| [nredis-proxy](https://github.com/wxmclub/nredis-proxy) | 12 | JAVA | a redis proxy based on netty. arch design. nredis-proxy 是一个以redis 协议为主的高性能稳定的代理中间件服务，不侵入业务代码，与业务毫无联系，不需要改任何应用代码，天然支持分布式部署。 |
| [predixy](https://github.com/joyieldInc/predixy) | 406 | C++ | A high performance and full features proxy for redis, support redis sentinel and redis cluster. |
| [onecache](https://github.com/onexsoft/onecache) | 216 | C++ | OneCache a Redis protocol based distributed cache middleware, as a replacement of Twemproxy or Codis. Unlike twemproxy, OneCache can offer 500,000 or higher QPS for single instance with lower latency.  |
| [redis-twemproxy-agent](https://github.com/Stono/redis-twemproxy-agent) | 84 | JavaScript | A simple nodejs application which will connect to Redis-Sentinel and monitor for the master-change event. It will then update TwemProxy (nutcracker) and restart it. |
| [r3proxy](https://github.com/ksarch-saas/r3proxy) | 22 | C | written by baidu tieba. a twemproxy with rediscluster support. |
| [meitu/twemproxy](https://github.com/meitu/twemproxy) | 124 | C | written by meitu. [meitu](https://github.com/meitu/) twemproxy is a multi-process, fast and lightweight proxy for [memcached](www.memcached.com) and [redis](redis.io) protocol. It was built primarily to reduce the number of connections to the caching servers on the backend. This, together with protocol pipelining and sharding enables you to horizontally scale your distributed caching architecture. |
| [clia/rcproxy](https://github.com/clia/rcproxy) | 31(until 2023/08/17) | Rust | RCProxy is a lightweight, fast but powerful Redis Cluster Proxy written in Rust |


---
## Redis Module

| Project Name | Stars | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [rediSQL](https://github.com/RedBeardLab/rediSQL) | 890 | Rust | Redis module that provides a completely functional SQL database |
| [redis-storage](https://github.com/qiye/redis-storage) | 264 | Lua | 把leveldb嵌入到redis实现真正的数据持久存储 |
| [RedisJSON](https://github.com/RedisJSON/RedisJSON) | 867 | C | a Redis module that implements ECMA-404 The JSON Data Interchange Standard as a native data type. It allows storing, updating and fetching JSON values from Redis keys (documents). |
| [RedisTimeSeries](https://github.com/RedisTimeSeries/RedisTimeSeries) | 208 | C | a Redis Module adding a Time Series data structure to Redis |

---
## Redis Client

| Project Name | Stars | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [hiredis-vip](https://github.com/vipshop/hiredis-vip) | 169(2019/03/24) | C | vip is a C client library for the Redis database, supported redis cluster, fully contained and based on Hiredis |
| [redispipe](https://github.com/joomcode/redispipe) | 54(2019/03/24) | Go | High-throughput Redis client for Go with implicit pipelining |
| [lettuce-core](https://github.com/lettuce-io/lettuce-core) | 2358 | Java | Lettuce is a scalable thread-safe Redis client for synchronous, asynchronous and reactive usage. Multiple threads may share one connection if they avoid blocking and transactional operations such as BLPOP and MULTI/EXEC. Lettuce is built with netty. Supports advanced Redis features such as Sentinel, Cluster, Pipelining, Auto-Reconnect and Redis data models. |
| [redis-tui](https://github.com/mylxsw/redis-tui) | 261(2019/04/28) | Go | A Redis Text-based UI client in CLI |
| [hiredis-py](https://github.com/redis/hiredis-py) | 336(2019/10/30) |  Python | Python extension that wraps protocol parsing code in hiredis. It primarily speeds up parsing of multi bulk replies. |
| [redis-rs](https://github.com/mitsuhiko/redis-rs) | 2000(2021/05/29) | Rust | a high level redis library for Rust. It provides convenient access to all Redis functionality through a very flexible but low-level API. It uses a customizable type conversion trait so that any operation can return results in just the type you are expecting. This makes for a very pleasant development experience. |
| [go-ycsb](https://github.com/pingcap/go-ycsb) | 509(2023/07/14) | Go | go-ycsb is a Go port of YCSB. It fully supports all YCSB generators and the Core workload so we can do the basic CRUD benchmarks with Go. |
| [eredis](https://github.com/Nordix/eredis) | 30(2023/07/14) | Erlang | Erlang Redis client. This is an actively maintained fork used and sponsored by Ericsson via Nordix Foundation.  |
|  [aedis](https://github.com/mzimbres/aedis)  |  145(2023/07/14)   |  C++  |  An async redis client designed for performance and scalability  |

---
## Redis Data Migration

| Project Name | Stars | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [RedisShake](https://github.com/alibaba/RedisShake) | 110 | Go | Redis-shake is a tool for synchronizing data between two redis databases |
| [redis-port](https://github.com/CodisLabs/redis-port) | 110 | C | parse redis rdb file, sync data between redis master and slave |
| [rdd](https://github.com/r043v/rdd) | 76 | C | redis database dumper, this tool can be used to dump a redis database, work on dump and put dump into redis this tool not use .rdb file! It's a beta software, use it at your own risk! |
| [redis-migrate-tool](https://github.com/vipshop/redis-migrate-tool) | 560 | C | redis-migrate-tool is a convenient and useful tool for migrating data between redis. It is based on redis replication. In the process of migrating data, the source redis also can provide services for users. |
| [redis rdb file splitter](http://blog.nosqlfan.com/html/4092.html) | | | In this Chinese blog you will get a script to split Redis rdb db file. |
| [redis-migration](https://github.com/helifu/redis-migration) | 52 | C |  redis-migration is a fast, light-weight migration tool for redis. Just add redis-migration.c to the redis sources. We scale out our redis clusters by this tool. Star: 35(until 2017/08/22). |
| [Bifrost](https://github.com/brokercap/Bifrost) | 1700(until 20231203) |  Go | transfer data from MySQL,MariaDB,kafka to Redis,MongoDB,ClickHouse,StarRocks,Doris,Kafka |

---
## Redis Monitor

| Project Name | Stars(until 2019/04/14) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [RedisLive](https://github.com/nkrode/RedisLive) | 2845 | JavaScript | Visualize your redis instances, analyze query patterns and spikes. |
| [redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools) | 3103 | Python | Rdbtools is a parser for Redis' dump.rdb files. The parser generates events similar to an xml sax parser, and is very efficient memory wise. In addition, rdbtools provides utilities to :Generate a Memory Report of your data across all databases and keys; Convert dump files to JSON; Compare two dump files using standard diff tools. Rdbtools is written in Python, though there are similar projects in other languages. |
| [redmon](https://github.com/steelThread/redmon) | 1530 | Ruby | A web interface for managing redis: cli, admin, and live monitoring. Simple sinatra based dashboard for redis. After seeing the fnordmetric project I was inspired to write this. Some of the ideas there have be carried over here. |
| [redis-faina](https://github.com/facebookarchive/redis-faina) | 1407 | Python | At its core, redis-faina uses the Redis MONITOR command, which echoes every single command (with arguments) sent to a Redis instance. It parses these entries, and aggregates stats on the most commonly-hit keys, the queries that took up the most amount of time, and the most common key prefixes as well. |
| [redis-stat](https://github.com/junegunn/redis-stat) | 1761 | Ruby | redis-stat is a simple Redis monitoring tool written in Ruby.It is based on INFO command of Redis, and thus generally won't affect the performance of the Redis instance unlike the other monitoring tools based on MONITOR command.redis-stat allows you to monitor Redis instances either with vmstat-like output from the terminal or with the dashboard page served by its embedded web server. |
| [redispapa](https://github.com/no13bus/redispapa) | 378 | Python | another redis monitor by using flask, angular, socket.io. we use redis info to monitor the redis usage. PAPA means a father who is monitoring the redis. accoding to the redis doc, it is be recommanded to use info other than monitor. |
| [redis-monitor](https://github.com/LittlePeng/redis-monitor) | 483 | JavaScript | base RedisLive,monitor multiple redis-server in product enviroment: monitor multiple redis-instance in one page; monitor memory,comand per sec,HitRate,keyspace, master-slave change,expire; sms alert when crash , master-slave stats changed. |
| [redis-sampler](https://github.com/antirez/redis-sampler) | 219 | Ruby | Small program to understand the composition of your Redis data set. |
| [redis-audit](https://github.com/snmaynard/redis-audit) | 221 | Ruby | This script samples a number of the Redis keys in a database and then groups them with other similar looking keys. It then displays key metrics around those groups of keys to help you spot where efficiencies can be made in the memory usage of your Redis database.Warning: The script cannot be used with AWS Elasticache Redis instances, as the debug command is restricted. |
| [redis_key_sizes.sh](https://gist.github.com/epicserve/5699837) | 125 | shell | A simple script to print the size of all your Redis keys. |
| [redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools) | 3103 | Python | Rdbtools is a parser for Redis' dump.rdb files. The parser generates events similar to an xml sax parser, and is very efficient memory wise. |
| [redis-full-check](https://github.com/alibaba/RedisFullCheck) | 76 | Go | Redis-full-check is developed and maintained by NoSQL Team in Alibaba-Cloud Database department. Redis-full-check performs full data verification by comparing the data of the source database and the destination database. |
| [redis-inventory](https://github.com/obukhov/redis-inventory) | 58 | Go |  Redis inventory is a tool to analyse Redis memory usage by key patterns and displaying it hierarchically. The name is inspired by "Disk Inventory X" tool doing similar analysis for disk usage. |
| [rdr](https://github.com/xueqiu/rdr) | 1000 | Go | a tool to parse redis rdbfile. Comparing to redis-rdb-tools, RDR is implemented by golang, much faster (5GB rdbfile takes about 2mins on my PC). |

---
## Redis Admin Web & UI


| Project Name | Stars(until 2019/04/16) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [overlord](https://github.com/bilibili/overlord) | 236 | Go | 哔哩哔哩基于Go语言编写的基于memcache和redis&redis-cluster高可用的缓存服务解决方案 |
| [RedisDesktopManager](https://github.com/uglide/RedisDesktopManager) | 11780 | C++ | Redis Desktop Manager (aka RDM)— is a cross-platform open source Redis DB management tool (i.e. Admin GUI). Redis Desktop Manager developed to replace hundreds of slow and ugly tools for redis. |
| [redmon](https://github.com/steelThread/redmon) | 1530 | Ruby | A web interface for managing redis: cli, admin, and live monitoring. Simple sinatra based dashboard for redis. After seeing the fnordmetric project I was inspired to write this. Some of the ideas there have be carried over here. |
| [cachecloud](https://github.com/sohutv/cachecloud) | 4079 | Java | A private redis cloud platform developed by Sohu Inc. |
| [django-redisboard](https://github.com/ionelmc/django-redisboard) | 207 | Python | Redis monitoring and inspection tool in django admin.its features: Sever statistics in the admin changelist; Key summary in the inspect view; Value introspection with pagination for lists and sorted sets. |
| [RedisReact](https://github.com/ServiceStackApps/RedisReact) | 302 | JavaScript | Redis React is a simple user-friendly UI for browsing data in Redis servers which takes advantages of the complex type conventions built in the ServiceStack.Redis Client to provide a rich, human-friendly UI for navigating related datasets, enabling a fast and fluid browsing experience for your Redis servers. Its related project is ServiceStack.Redis. |
| [redis-ctl](https://github.com/projecteru/redis-ctl) | 127 | Python | Redis Instance Controlling and Distribution Service. |
| [fastoredis](https://github.com/fastogt/fastoredis) | 270 | |  FastoRedis is a crossplatform Redis GUI management tool. |
| [Redsmin](https://www.redsmin.com/) | || a developer oriented online administration and monitoring service for Redis and Redis cluster. Redsmin is trusted by more than 10K developers world-wide and manage thousands of Redis servers in real-time. |
| [RedisManager](https://github.com/giuseppesalvo/RedisManager) | 10 | Swift | Simple Mac Application to manage Redis Server.  |
| [redisvo](https://github.com/taomin597715379/redisvo) | 27 | JavaScript | a web-based redis data visualization tool。|
| [medis](https://github.com/luin/medis) | 7352 | JavaScript |  Medis is a beautiful, easy-to-use Redis management application built on the modern web with Electron, React, and Redux. It's powered by many awesome Node.js modules, especially ioredis and ssh2. |
| [AnotherRedisDesktopManager](https://github.com/qishibo/AnotherRedisDesktopManager) | 18000 | JavaScript | A faster, better and more stable redis desktop manager [GUI client], compatible with Linux, Windows, Mac. What's more, it won't crash when loading massive keys. |
| [RedisInsight](https://github.com/RedisInsight/RedisInsight) | 3300(2023/07/14) | Js | RedisInsight is a visual tool that provides capabilities to design, develop and optimize your Redis application. Query, analyse and interact with your Redis data. |

---
## Redis Golang Packages

| Project Name | Stars(until 2019/04/16) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [redigo](https://github.com/garyburd/redigo/) | 66 | Go | Redis Sentinel support for redigo library. |
| [redigomock](https://github.com/rafaeljusto/redigomock) | 96 | Go | Easy way to unit test projects using redigo library (Redis client in go). |
| [redi-go-cluster](https://github.com/chasex/redis-go-cluster) | 291 | Go | redis-go-cluster is a golang implementation of redis client based on Gary Burd's Redigo. It caches slot info at local and updates it automatically when cluster change. The client manages a connection pool for each node, uses goroutine to execute as concurrently as possible, which leads to its high efficiency and low lantency. |
| [go-sentinel](https://github.com/FZambia/go-sentinel) | 33 | Go | Redis Sentinel support for redigo library. |
| [redis-failover](https://github.com/FZambia/go-sentinel) | 66 | Go | Automatic redis monitoring and failover based on Go. |
| [miniredis](https://github.com/alicebob/miniredis) | 635 | Go | Pure Go Redis test server, used in Go unittests. Sometimes you want to test code which uses Redis, without making it a full-blown integration test. Miniredis implements (parts of) the Redis server, to be used in unittests. |
| [redeo](https://github.com/bsm/redeo) | 246 | Go | High-performance framework for building redis-protocol compatible TCP servers/services. Optimised for speed! |
| [libredis](https://github.com/therealbill/libredis) | 10 | Go | Libredis is intended to be more than a simple client connection library. It will include Redis specific custom operations, Structures, and capabilities suitable for integrating with any Go code which interacts with Redis ranging from simple CRUD operations to service management. |
| [go-redis](https://github.com/fiorix/go-redis) | 41 | Go | go-redis is a Redis client library for the Go programming language. It's built on the skeleton of gomemcache. |
| [goatee](https://github.com/johnernaut/goatee) | 269 | Go | A Redis-backed notification server written in Go. goatee works by listening on a channel via Redis Pub/Sub and then sending the received message to connected clients via WebSockets. Clients may create channels to listen on by using the goatee client library. |
| [juggler](https://github.com/mna/juggler) | 65 | Go | Juggler implements highly decoupled, asynchronous RPC and pub-sub over websocket connections using redis as broker. It refers both to a websocket subprotocol and the implementation of a juggler server. The repository also contains implementations of the callee, broker and client roles. This is still experimental. Use at your own risk. Not battle-tested in production environment. API may change. Javascript (and other languages) client not implemented yet. |
| [broadcaster](https://github.com/rubenv/broadcaster) | 24 | Go | Package broadcaster implements a websocket server for broadcasting Redis pub/sub messages to web clients. |
| [redisocket.v2](https://github.com/syhlion/redisocket.v2) | 1 | Go | Base on gorilla/websocket & garyburd/redigo. |
| [redis](https://github.com/go-redis/redis) | 5486 | Go | Redis client for Golang. |
| [Go-Redis](https://github.com/alphazero/Go-Redis) | 389 | Go | Google Go Client and Connectors for Redis. |
| [gosexy/redis](https://github.com/gosexy/redis) | 168 | Go | Redis client for Go that maps the full redis command list into equivalent Go functions. |
| [go-resp3](https://github.com/stfnmllr/go-resp3) | 11 | Go | Google Go Redis RESP3 client |
| [rueidis](https://github.com/rueian/rueidis) | 447(2022/08/07) | Go | A Fast Golang Redis RESP3 client that supports Client Side Caching, Auto Pipelining, Generics OM, RedisJSON, RedisBloom, RediSearch, RedisAI, RedisGears, etc. |
| [redis_rate](https://github.com/go-redis/redis_rate) | 620(2023/07/14) | Go | This package is based on rwz/redis-gcra and implements GCRA (aka leaky bucket) for rate limiting based on Redis.  |

---
## Redis Based Lock&Cache
| Project Name | Stars(until 2019/04/16) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [disgear](https://github.com/yangbutao/disgear) | 77 | Java | Disgear is a distributed cache based on redis, support data segmentation on multiple machines, support HA, write&read separation ,and automatic election support the master node failure. There is also a [Chinese translation version](http://www.rigongyizu.com/distributed-locks-using-redis/) of this blog. |
| [Distributed locks using Redis](https://engineering.gosquared.com/distributed-locks-using-redis) | | | How to create reliable locks for a distributed architecture. |
| [Redis lock algorithm and implementation list: Distributed locks with Redis](https://redis.io/topics/distlock) | | |  |
| [redsync](https://github.com/go-redsync/redsync) | 358 | Go | Distributed mutual exclusion lock using Redis for Go. |

---
## Redis Ecosystem
| Project Name | Stars(until 2019/04/16) | Lang | Description |
| :----------- | :---- | :--- | :---------- |
| [awesome-redis](https://github.com/zhemingwang/awesome-redis) | 330 | | A curated list of amazingly awesome redis and redis ecosystem resources. |
| [RedisWeekly](http://redisweekly.com) | | | A once–weekly e-mail round-up of Redis news, articles, tools and libraries followed by more than 5 000 Redis developers. |

---
* written by Alex Stocks on 2016/03/22

>- add redmon & redispapa & django-redisboard on 2016/04/15
>- add Redsmin & RedisManager & RedisWeekly on 2016/04/19
>- add twemproxies & fastoredis on 2016/04/20
>- add redis cluster(codis & Pika) on 2016/05/12
>- add redigo & redi-go-cluster & redigomock & go-sentinel on 2016/06/09
>- add ardb & twemproxy-163 on 2016/09/02
>- add Pedis & redis-failover & miniredis & redeo & libredis & go-redis on 2016/09/23
>- add goatee & juggler & broadcaster & redisocket.v2 on 2016/10/02
>- add redis on 2016/10/03
>- add Go-Redis & Pushlet on 2016/10/24
>- add xredis-server on 2016/11/16
>- add x-pipe on 2017/07/01
>- add redisvo on 2017/08/10
>- add gosexy/redis on 2017/08/12
>- add medis on 2017/08/15
>- add qdb & redsync && cc on 2017/08/19
>- add redis-rdb-tools & redis-migration & vire & twemproxy-vip & hiredis-vip & nredis-proxy on 2017/08/22
>- add predixy on 2017/08/27
>- add onecache on 2017/09/04
>- add swapdb on 2017/09/08
>- add redis-twemproxy-agent on 2017/09/22
>- add ApsaraCache on 2017/10/14
>- add r3proxy on 2018/05/16
>- add [meitu/twemproxy](https://github.com/meitu/twemproxy)  on 2018/09/07
>- add [titan](https://github.com/meitu/titan) on 2018/12/12
>- add [KeyDB](https://github.com/JohnSully/KeyDB) & [redis-full-check](https://github.com/aliyun/redis-full-check) on 2019/03/13
>- add [rediSQL](https://github.com/RedBeardLab/rediSQL) & [aster](https://github.com/wayslog/aster) on 2019/03/24
>- add [undermoon](https://github.com/doyoubi/undermoon) on 2019/04/05
>- add [RedisShake](https://github.com/alibaba/RedisShake) & [lettuce-core](https://github.com/lettuce-io/lettuce-core) on 2019/04/06
>- add [overlord](https://github.com/bilibili/overlord) on 2019/04/10
>- add [redis-tui](https://github.com/mylxsw/redis-tui) on 2019/04/28
>- add [rsedis](https://github.com/seppo0010/rsedis) on 2019/07/01
>- add [RedisJSON](https://github.com/RedisJSON/RedisJSON) on 2019/09/05
>- add [RedisTimeSeries](https://github.com/RedisTimeSeries/RedisTimeSeries) on 2019/09/11
>- add [hiredis-py](https://github.com/redis/hiredis-py) on 2019/09/17
>- add [go-resp3](https://github.com/stfnmllr/go-resp3)  on 2020/07/22
>- add [redis-windows](https://github.com/ServiceStack/redis-windows)  on 2020/08/20
>- add [Tendis](https://github.com/tencent/Tendis) on 2020/12/24
>- add [redis-rs](https://github.com/mitsuhiko/redis-rs) on 2021/05/29
>- add [godis](https://github.com/HDT3213/godis) on 2021/06/22
>- add [redis-inventory](https://github.com/obukhov/redis-inventory) on 2021/09/16
>- add [AnotherRedisDesktopManager](https://github.com/qishibo/AnotherRedisDesktopManager) on 2022/01/05
>- add [rueidis](https://github.com/rueian/rueidis) on 2022/08/06
>- add [rdr](https://github.com/xueqiu/rdr) & [dragonfly](https://github.com/dragonflydb/dragonfly) on 2023/04/16
>- add [redis-operator](https://github.com/OT-CONTAINER-KIT/redis-operator) & [go-ycsb](https://github.com/pingcap/go-ycsb) & [eredis](https://github.com/Nordix/eredis) & [aedis](https://github.com/mzimbres/aedis) & [RedisInsight](https://github.com/RedisInsight/RedisInsight) & [redis_rate](https://github.com/go-redis/redis_rate) on 2023/07/14
 >- add [clia/rcproxy](https://github.com/clia/rcproxy) & [rsedis](https://github.com/seppo0010/rsedis)  on 2023/08/17
 >- add Bifrost](https://github.com/brokercap/Bifrost) on 2023/12-03

