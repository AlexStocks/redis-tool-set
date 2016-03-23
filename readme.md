# Redis tool list #

Here is a Redis tool list. I hope you will find one or two of them that you'd like to try out.

- [Redis tool list](#redis tool list)
	- [Redis Variety](#redis variety)
	- [Redis Proxy](#redis proxy)
	- [Redis Data Migration](#redis data migration)
	- [Redis Monitor](#redis monitor)
	- [Redis Admin Web UI](#redis admin web ui)
	- [Redis Ecosystem](#redis ecosystem)

---
## Redis Variety
* [webdis](https://github.com/nicolasff/webdis) - A very simple web server providing an HTTP interface to Redis. It uses hiredis, jansson, libevent, and [http-parser](https://github.com/nodejs/http-parser). star: 1595.
* [Qedis](https://github.com/loveyacper/Qedis) - A C++11 implementation of Redis server. star: 4.
* [AliRedis](http://blog.sina.com.cn/s/blog_e59371cc0101br74.html) - AliRedis, which is developed by Alibaba， use a new nginx-like(one-master-multi-worker) framework, in order to get full use of the CPU cores.

---
## Redis Proxy
* [bilitw](https://github.com/anewhuahua/bilitw) - bilitw (bilibili twemproxy), which introduce multi process of twemproxy(one master and mutli worker), is order to get full use of the CPU cores. star: 27.
* [Corvus](https://github.com/eleme/corvus) - A fast and lightweight Redis Cluster Proxy for Redis 3.0. star: 26.
* [twemproxy](https://github.com/twitter/twemproxy) - A fast, light-weight proxy for memcached and redis. star: 5123.

---
## Redis Data Migration
* [redis-port](https://github.com/CodisLabs/redis-port) - parse redis rdb file, sync data between redis master and slave. star: 80.
* [redis-migration](http://www.bitstech.net/2016/03/03/redis-migration/) - A Chinese blog declares its tool(redis-migration, developed by Netease Inc.) is better than redis-port and not open source.
* [redis rdb file splitter](http://blog.nosqlfan.com/html/4092.html) - In this Chinese blog you will get a script to split Redis rdb db file.

---
## Redis Monitor
* [redis-rdb-tools](https://github.com/sripathikrishnan/redis-rdb-tools) - Rdbtools is a parser for Redis' dump.rdb files. The parser generates events similar to an xml sax parser, and is very efficient memory wise.
In addition, rdbtools provides utilities to :Generate a Memory Report of your data across all databases and keys; Convert dump files to JSON; Compare two dump files using standard diff tools. Rdbtools is written in Python, though there are similar projects in other languages. star: 1471.
* [redis-faina](https://github.com/facebookarchive/redis-faina) - At its core, redis-faina uses the Redis MONITOR command, which echoes every single command (with arguments) sent to a Redis instance. It parses these entries, and aggregates stats on the most commonly-hit keys, the queries that took up the most amount of time, and the most common key prefixes as well. star：1002.
* [redis-stat](https://github.com/junegunn/redis-stat) - redis-stat is a simple Redis monitoring tool written in Ruby.It is based on INFO command of Redis, and thus generally won't affect the performance of the Redis instance unlike the other monitoring tools based on MONITOR command.redis-stat allows you to monitor Redis instances either with vmstat-like output from the terminal or with the dashboard page served by its embedded web server. star: 823.
* [redis-monitor](https://github.com/LittlePeng/redis-monitor) - base RedisLive,monitor multiple redis-server in product enviroment: monitor multiple redis-instance in one page; monitor memory,comand per sec,HitRate,keyspace, master-slave change,expire; sms alert when crash , master-slave stats changed. star: 179.
* [redis-sampler](https://github.com/antirez/redis-sampler) - Small program to understand the composition of your Redis data set. star: 179.
* [redis-audit](https://github.com/snmaynard/redis-audit) - This script samples a number of the Redis keys in a database and then groups them with other similar looking keys. It then displays key metrics around those groups of keys to help you spot where efficiencies can be made in the memory usage of your Redis database.Warning: The script cannot be used with AWS Elasticache Redis instances, as the debug command is restricted. star: 114.
* [redis_key_sizes.sh](https://gist.github.com/epicserve/5699837) - A simple script to print the size of all your Redis keys. star: 52.

---
## Redis Admin Web UI
* [RedisDesktopManager](https://github.com/uglide/RedisDesktopManager) - Redis Desktop Manager (aka RDM)— is a cross-platform open source Redis DB management tool (i.e. Admin GUI). Redis Desktop Manager developed to replace hundreds of slow and ugly tools for redis. star: 2557.
* [RedisLive](https://github.com/nkrode/RedisLive) - Visualize your redis instances, analyze query patterns and spikes. star: 2125.
* [cachecloud](https://github.com/sohutv/cachecloud) - A private redis cloud platform developed by Sohu Inc. star: 717.
* [RedisReact](https://github.com/ServiceStackApps/RedisReact) - Redis React is a simple user-friendly UI for browsing data in Redis servers which takes advantages of the complex type conventions built in the ServiceStack.Redis Client to provide a rich, human-friendly UI for navigating related datasets, enabling a fast and fluid browsing experience for your Redis servers. Its related project is [ServiceStack.Redis](https://github.com/ServiceStack/ServiceStack.Redis). star: 81.

---
## Redis Based Lock&Cache
* [disgear](https://github.com/yangbutao/disgear) - [Disgear](http://m.blog.csdn.net/article/details?id=16896669) is a distributed cache based on redis, support data segmentation on multiple machines, support HA, write&read separation ,and automatic election support the master node failure. star: 53.
* [Distributed locks using Redis](https://engineering.gosquared.com/distributed-locks-using-redis) - How to create reliable locks for a distributed architecture. There is also a [Chinese translation version](http://www.rigongyizu.com/distributed-locks-using-redis/) of this blog.
* [Redis lock algorithm and implementation list: Distributed locks with Redis](http://redis.io/topics/distlock)

---
## Redis Ecosystem
* [awesome-redis](https://github.com/zhemingwang/awesome-redis) - A curated list of amazingly awesome redis and redis ecosystem resources. star: 80.

---
*written by Alex Stocks on 2016/03/22*