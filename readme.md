# Redis tool list #

Here is a Redis tool list. I hope you will find one or two of them that you'd like to try out.


Table of Contents
=================
  * [Redis Cluster](#redis-cluster)
  * [Redis Variety](#redis-variety)
  * [Redis Proxy](#redis-proxy)
  * [Redis Client](#redis-client)
  * [Redis Data Migration](#redis-data-migration)
  * [Redis Monitor](#redis-monitor)
  * [Redis Admin Web &amp; UI](#redis-admin-web--ui)
  * [Redis Golang Packages](#redis-golang-packages)
  * [Redis Based Lock&amp;Cache](#redis-based-lockcache)
  * [Redis Ecosystem](#redis-ecosystem)

---
## Redis Cluster
* [Codis](https://github.com/CodisLabs/codis) - Codis is a proxy based high performance Redis cluster solution written in Go. It is production-ready and widely used at wandoujia.com and many companies. star: 4177(until 2016/05/12).
* [Pika](https://github.com/Qihoo360/pika) - [Pika](https://mp.weixin.qq.com/s?__biz=MzAwMDU1MTE1OQ==&mid=2653547160&idx=1&sn=befd195e2aa788775aaf1cc3b6f6fab3&scene=1&srcid=05125RMahWYSgUb4fIUJYIj5&pass_ticket=fV%2BqHxDSZBGR5J2M0sWKaCnKGlnuoGkHfFfqcHa5mu0Lw4yA4wUZoRAqV7CQuMMk#rd) is a nosql compatible with redis protocol, it is developed by Qihoo's DBA and infrastructure team, and it is widely used in QiHoo. Pika is a persistent huge storage service , compatible with the vast majority of redis interfaces (details), including string, hash, list, zset, set and management interfaces. With the huge amount of data stored, redis may suffer for a capacity bottleneck, and pika was born for solving it. Except huge storage capacity, pika also support master-slave mode by slaveof command, including full and partial synchronization. star:85(until 2016/05/12).
* [x-pipe](https://github.com/ctripcorp/x-pipe) -  Redis 多数据中心集群，一是为了提升可用性，解决数据中心 DR(Disaster Recovery) 问题，二是提升访问性能，每个数据中心可以读取当前数据中心的数据，无需跨机房读数据。star:284(until 2017/07/01).
* [cc](https://github.com/ksarch-saas/cc) - This is a Redis Cluster Controller to control the state of the cluster nodes and provide http api and tools(both command line and web ui). Star: 17(until 2017/08/19). Lang: go & Js.

---
## Redis Variety
* [webdis](https://github.com/nicolasff/webdis) - A very simple web server providing an HTTP interface to Redis. It uses hiredis, jansson, libevent, and [http-parser](https://github.com/nodejs/http-parser). star: 1595.
* [ardb](https://github.com/yinqiwen/ardb) - A redis protocol compatible nosql, it support multiple storage engines as backend like Google's LevelDB, Facebook's RocksDB, OpenLDAP's LMDB, PerconaFT, WiredTiger, ForestDB. star 739(until 2016/09/02).
* [Pedis](https://github.com/fastio/pedis) - NoSQL data store using the SEASTAR framework, compatible with REDIS. star:169(until 2016/09/23)
* [Qedis](https://github.com/loveyacper/Qedis) - A C++11 implementation of Redis server. star: 4.
* [AliRedis](http://blog.sina.com.cn/s/blog_e59371cc0101br74.html) - AliRedis, which is developed by Alibaba， use a new nginx-like(one-master-multi-worker) framework, in order to get full use of the CPU cores.
* [Pushlet](https://github.com/wjw465150/Pushlet/tree/branch-redis) - Pushlet 是一个开源的 Comet 框架,Pushlet 使用了观察者模型：客户端发送请求，订阅感兴趣的事件；服务器端为每个客户端分配一个会话 ID 作为标记，事件源会把新产生的事件以多播的方式发送到订阅者的事件队列里。(lang:js, star:79, 2016/10/24)
* [xredis-server](https://github.com/0xsky/xredis-server) - redis-server is a redis server framework library write by C++, using this library you can develop redis protocol compatible server easily. xredis-server requires libevent. star: 46(until 2016/11/16).
* [qdb](https://github.com/reborndb/qdb) - A fast, high availability, fully Redis compatible store engine. star: 287(until 2017/08/19).
* [vire](https://github.com/vipshop/vire) - vire (pronounced "vip-redis") is a multithread redis(based on redis-3.2.0) maintains in vipshop. star: 110(until 2017/08/22). Lang: C.

---
## Redis Proxy
* [twemproxy](https://github.com/twitter/twemproxy) - A fast, light-weight proxy for memcached and redis. star: 5123.
* [redis-cerberus](https://github.com/HunanTV/redis-cerberus) - A Redis cluster proxy. Its monitor tool is [redis-ctl](http://m.oschina.net/blog/377568). star: 189.
* [Redsmin proxy deamon](https://github.com/Redsmin/proxy) - Access local redis instance from Redsmin https://redsmin.com. Redsmin and Redsmin proxy communicate through a secure connection using the TLS 1.2 protocol so no one will be able to inspect the data looking at the traffic. star: 40(until 2016/04/19).
* [bilitw](https://github.com/anewhuahua/bilitw) - bilitw (bilibili twemproxy), which introduce multi process of twemproxy(one master and mutli worker), is order to get full use of the CPU cores. star: 27.
* [Corvus](https://github.com/eleme/corvus) - A fast and lightweight Redis Cluster Proxy for Redis 3.0. star: 26.
* [twemproxy-163](https://github.com/helifu/twemproxy-163) - twemproxy-163 supports redis-server failover by communicating with redis-sentinel. star: 16(until 2016/09/02).
* [twemproxies](https://github.com/vipshop/twemproxies) - twemproxies ( nutcrackers ) is a multithread, fast and lightweight proxy for memcached and redis protocol. It was built primarily to reduce the number of connections to the caching servers on the backend. This, together with protocol pipelining and sharding enables you to horizontally scale your distributed caching architecture. star: 2(until 2016/04/20).
* [twemproxy-vip](https://github.com/vipshop/twemproxy-vip) - twemproxy maintained and used at vipshop. star: 39(until 2017/08/22). Lang: C.
* [nredis-proxy](https://github.com/wxmclub/nredis-proxy) - a redis proxy based on netty. [arch design](https://mp.weixin.qq.com/s?__biz=MzI3MzEzMDI1OQ==&mid=2651816198&idx=1&sn=306153cb467010d2f5af31260ac6e694&chksm=f0dcd77ac7ab5e6c5f385756abc4853f8bccc1311c98120e3ce4c3abb9ab2c168b82a60d187b&mpshare=1&scene=1&srcid=0217Dk1nMM0pxGJQqvjug02Z&pass_ticket=seR%2BdnRh98xppQGWjIyfOL%2BpIIVEd1myAxSbNwoG7bNljwB2RhgnvuL1L%2F5V7tpy#rd). star: 6(until 2017/08/22). Lang: Java.
* [predixy](https://github.com/joyieldInc/predixy) - A high performance and full features proxy for redis, support redis sentinel and redis cluster. star: 50(until 2017/08/27). Lang: C++.
* [onecache](https://github.com/onexsoft/onecache) - OneCache a Redis protocol based distributed cache middleware, as a replacement of Twemproxy or Codis. Unlike twemproxy, OneCache can offer 500,000 or higher QPS for single instance with lower latency. star: 195(until 2017/09/04). Lang: C++.

---
## Redis Client
* [hiredis-vip](https://github.com/vipshop/hiredis-vip) - Hiredis-vip is a C client library for the Redis database, supported redis cluster, fully contained and based on Hiredis. star: 91(until 2017/08/22). Lang: C.

---
## Redis Data Migration
* [redis-port](https://github.com/CodisLabs/redis-port) - parse redis rdb file, sync data between redis master and slave. star: 80.
* [rdd](https://github.com/r043v/rdd) - redis database dumper, this tool can be used to dump a redis database, work on dump and put dump into redis this tool not use .rdb file! It's a beta software, use it at your own risk! star: 58.
* [redis-migrate-tool](https://github.com/vipshop/redis-migrate-tool) - redis-migrate-tool is a convenient and useful tool for migrating data between redis. It is based on redis replication. In the process of migrating data, the source redis also can provide services for users. star: 19.
* [redis rdb file splitter](http://blog.nosqlfan.com/html/4092.html) - In this Chinese blog you will get a script to split Redis rdb db file.
* [redis-migration](https://github.com/helifu/redis-migration) - redis-migration is a fast, light-weight migration tool for redis. Just add redis-migration.c to the redis sources. We scale out our redis clusters by this tool. Star: 35(until 2017/08/22). Lang: C.

---
## Redis Monitor 
* [RedisLive](https://github.com/nkrode/RedisLive) - Visualize your redis instances, analyze query patterns and spikes. star: 2125.
* [redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools) - Rdbtools is a parser for Redis' dump.rdb files. The parser generates events similar to an xml sax parser, and is very efficient memory wise.
In addition, rdbtools provides utilities to :Generate a Memory Report of your data across all databases and keys; Convert dump files to JSON; Compare two dump files using standard diff tools. Rdbtools is written in Python, though there are similar projects in other languages. star: 1471.
* [redmon](https://github.com/steelThread/redmon) - A web interface for managing redis: cli, admin, and live monitoring. Simple sinatra based dashboard for redis. After seeing the fnordmetric project I was inspired to write this. Some of the ideas there have be carried over here. star: 1303 (until 2016/04/15).
* [redis-faina](https://github.com/facebookarchive/redis-faina) - At its core, redis-faina uses the Redis MONITOR command, which echoes every single command (with arguments) sent to a Redis instance. It parses these entries, and aggregates stats on the most commonly-hit keys, the queries that took up the most amount of time, and the most common key prefixes as well. star：1002.
* [redis-stat](https://github.com/junegunn/redis-stat) - redis-stat is a simple Redis monitoring tool written in Ruby.It is based on INFO command of Redis, and thus generally won't affect the performance of the Redis instance unlike the other monitoring tools based on MONITOR command.redis-stat allows you to monitor Redis instances either with vmstat-like output from the terminal or with the dashboard page served by its embedded web server. star: 823.
* [redispapa](https://github.com/no13bus/redispapa) - another redis monitor by using flask, angular, socket.io. we use redis info to monitor the redis usage. PAPA means a father who is monitoring the redis. accoding to the redis doc, it is be recommanded to use info other than monitor.
 star: 293(2016/04/15).
* [redis-monitor](https://github.com/LittlePeng/redis-monitor) - base RedisLive,monitor multiple redis-server in product enviroment: monitor multiple redis-instance in one page; monitor memory,comand per sec,HitRate,keyspace, master-slave change,expire; sms alert when crash , master-slave stats changed. star: 179.
* [redis-sampler](https://github.com/antirez/redis-sampler) - Small program to understand the composition of your Redis data set. star: 179.
* [redis-audit](https://github.com/snmaynard/redis-audit) - This script samples a number of the Redis keys in a database and then groups them with other similar looking keys. It then displays key metrics around those groups of keys to help you spot where efficiencies can be made in the memory usage of your Redis database.Warning: The script cannot be used with AWS Elasticache Redis instances, as the debug command is restricted. star: 114.
* [redis_key_sizes.sh](https://gist.github.com/epicserve/5699837) - A simple script to print the size of all your Redis keys. star: 52.
* [Datadog:how_to_collect/monitor_redis_metrics.md](https://github.com/AlexStocks/the-monitor/tree/master/redis) - Markdown files of Datadog : how to collect/monitor redis metrics. star: 37.
* [redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools) - Rdbtools is a parser for Redis' dump.rdb files. The parser generates events similar to an xml sax parser, and is very efficient memory wise. star: 2113(until 2017/08/22). Lang: Python.

---
## Redis Admin Web & UI 
* [RedisDesktopManager](https://github.com/uglide/RedisDesktopManager) - Redis Desktop Manager (aka RDM)— is a cross-platform open source Redis DB management tool (i.e. Admin GUI). Redis Desktop Manager developed to replace hundreds of slow and ugly tools for redis. star: 2557.
* [redmon](https://github.com/steelThread/redmon) - A web interface for managing redis: cli, admin, and live monitoring. Simple sinatra based dashboard for redis. After seeing the fnordmetric project I was inspired to write this. Some of the ideas there have be carried over here. star: 1303 (until 2016/04/15).
* [cachecloud](https://github.com/sohutv/cachecloud) - A private redis cloud platform developed by Sohu Inc. star: 717.
* [django-redisboard](https://github.com/ionelmc/django-redisboard) - Redis monitoring and inspection tool in django admin.its features: Sever statistics in the admin changelist; Key summary in the inspect view; Value introspection with pagination for lists and sorted sets. star: 174(until: 2016/04/15).
* [RedisReact](https://github.com/ServiceStackApps/RedisReact) - Redis React is a simple user-friendly UI for browsing data in Redis servers which takes advantages of the complex type conventions built in the ServiceStack.Redis Client to provide a rich, human-friendly UI for navigating related datasets, enabling a fast and fluid browsing experience for your Redis servers. Its related project is [ServiceStack.Redis](https://github.com/ServiceStack/ServiceStack.Redis). star: 81.
* [redis-ctl](https://github.com/HunanTV/redis-ctl) - Redis Instance Controlling and Distribution Service. star: 53.
* [fastoredis](https://github.com/fastogt/fastoredis) - FastoRedis is a crossplatform Redis GUI management tool. star: 42(until 2016/04/20).
* [Redsmin](https://www.redsmin.com) - a developer oriented online administration and monitoring service for Redis and Redis cluster. Redsmin is trusted by more than 10K developers world-wide and manage thousands of Redis servers in real-time.
* [RedisManager](https://github.com/giuseppesalvo/RedisManager) - Simple Mac Application to manage Redis Server. star: 6(until 2016/04/19).
* [redisvo](https://github.com/taomin597715379/redisvo) - a web-based redis data visualization tool。Star: 10(until 2017/08/10). Lang: Golang.
* [medis](https://github.com/luin/medis) - Medis is a beautiful, easy-to-use Redis management application built on the modern web with Electron, React, and Redux. It's powered by many awesome Node.js modules, especially ioredis and ssh2.Star: 4490(until 2017/08/15). Lang: Js.

---
## Redis Golang Packages 
* [redigo](https://github.com/garyburd/redigo/) - Redis Sentinel support for redigo library. star: 2236(until 2016/06/09).
* [redigomock](https://github.com/rafaeljusto/redigomock) - Easy way to unit test projects using redigo library (Redis client in go). star: 26(until 2016/06/09).
* [redi-go-cluster](https://github.com/chasex/redis-go-cluster) - redis-go-cluster is a golang implementation of redis client based on Gary Burd's Redigo. It caches slot info at local and updates it automatically when cluster change. The client manages a connection pool for each node, uses goroutine to execute as concurrently as possible, which leads to its high efficiency and low lantency. star: 50(until 2016/06/09).
* [go-sentinel](https://github.com/FZambia/go-sentinel) - Redis Sentinel support for redigo library. star: 5(until 2016/06/09).
* [redis-failover](https://github.com/FZambia/go-sentinel) - Automatic redis monitoring and failover based on Go.(http://siddontang.com/2015/05/03/use-hashicorp-raft-to-build-a-redis-sentinel/)(lang:golang, star:66, 2016/09/23).
* [miniredis](https://github.com/alicebob/miniredis) - Pure Go Redis test server, used in Go unittests. Sometimes you want to test code which uses Redis, without making it a full-blown integration test. Miniredis implements (parts of) the Redis server, to be used in unittests.(lang:golang, star:294, 2016/09/23)
* [redeo](https://github.com/bsm/redeo) - High-performance framework for building redis-protocol compatible TCP servers/services. Optimised for speed!(lang:golang, star:108, 2016/09/23)
* [libredis](https://github.com/therealbill/libredis) - Libredis is intended to be more than a simple client connection library. It will include Redis specific custom operations, Structures, and capabilities suitable for integrating with any Go code which interacts with Redis ranging from simple CRUD operations to service management.(lang:golang, star:8, 2016/09/23)
* [go-redis](https://github.com/fiorix/go-redis) - go-redis is a Redis client library for the Go programming language. It's built on the skeleton of gomemcache.(lang:golang, star:39, 2016/09/23)
* [goatee](https://github.com/johnernaut/goatee) - A Redis-backed notification server written in Go. goatee works by listening on a channel via Redis Pub/Sub and then sending the received message to connected clients via WebSockets. Clients may create channels to listen on by using the goatee client library.(lang:golang, star:270, 2016/10/02).
* [juggler](https://github.com/PuerkitoBio/juggler) - Juggler implements highly decoupled, asynchronous RPC and pub-sub over websocket connections using redis as broker. It refers both to a websocket subprotocol and the implementation of a juggler server. The repository also contains implementations of the callee, broker and client roles. This is still experimental. Use at your own risk. Not battle-tested in production environment. API may change. Javascript (and other languages) client not implemented yet.(lang:golang, star:41, 2016/10/02).
* [broadcaster](https://github.com/rubenv/broadcaster) - Package broadcaster implements a websocket server for broadcasting Redis pub/sub messages to web clients.(lang:golang, star:4, 2016/10/02).
* [redisocket.v2](https://github.com/syhlion/redisocket.v2) - Base on gorilla/websocket & garyburd/redigo.(lang:golang, star:0, 2016/10/02).
* [redis](https://github.com/go-redis/redis) - Redis client for Golang.(lang:golang, star:1109, 2016/10/03)
* [Go-Redis](https://github.com/alphazero/Go-Redis) - Google Go Client and Connectors for Redis.(lang:golang, star:238, 2016/10/24)
* [gosexy/redis](https://github.com/gosexy/redis) - Redis client for Go that maps the full redis command list into equivalent Go functions.(lang:golang, star:159, 2017/08/12)

---
## Redis Based Lock&Cache 
* [disgear](https://github.com/yangbutao/disgear) - [Disgear](http://m.blog.csdn.net/article/details?id=16896669) is a distributed cache based on redis, support data segmentation on multiple machines, support HA, write&read separation ,and automatic election support the master node failure. star: 53.
* [Distributed locks using Redis](https://engineering.gosquared.com/distributed-locks-using-redis) - How to create reliable locks for a distributed architecture. There is also a [Chinese translation version](http://www.rigongyizu.com/distributed-locks-using-redis/) of this blog.
* [Redis lock algorithm and implementation list: Distributed locks with Redis](http://redis.io/topics/distlock)
* [redsync](https://github.com/go-redsync/redsync) - Distributed mutual exclusion lock using Redis for Go. Star: 86 (until 2017/08/19). Lang: Golang.

---
## Redis Ecosystem 
* [awesome-redis](https://github.com/zhemingwang/awesome-redis) - A curated list of amazingly awesome redis and redis ecosystem resources. star: 80.
* [RedisWeekly](http://redisweekly.com) - A once–weekly e-mail round-up of Redis news, articles, tools and libraries followed by more than 5 000 Redis developers.

---
* written by Alex Stocks on 2016/03/22
* add redmon & redispapa & django-redisboard on 2016/04/15
* add Redsmin & RedisManager & RedisWeekly on 2016/04/19
* add twemproxies & fastoredis on 2016/04/20
* add redis cluster(codis & Pika) on 2016/05/12
* add redigo & redi-go-cluster & redigomock & go-sentinel on 2016/06/09
* add ardb & twemproxy-163 on 2016/09/02
* add Pedis & redis-failover & miniredis & redeo & libredis & go-redis on 2016/09/23
* add goatee & juggler & broadcaster & redisocket.v2 on 2016/10/02
* add redis on 2016/10/03
* add Go-Redis & Pushlet on 2016/10/24
* add xredis-server on 2016/11/16
* add x-pipe on 2017/07/01
* add redisvo on 2017/08/10
* add gosexy/redis on 2017/08/12
* add medis on 2017/08/15
* add qdb & redsync && cc on 2017/08/19
* add redis-rdb-tools & redis-migration & vire & twemproxy-vip & hiredis-vip & nredis-proxy on 2017/08/22
* add predixy on 2017/08/27
* add onecache on 2017/09/04