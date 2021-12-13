## Redis

* do not use default java Serializable (json with kotlinx.serialization is a good alternative)
* activate connection keep-alive (not by default) 'socketOptions(SocketOptions.builder().keepAlive(true).build())'
* offload cpu intensive operations to a dedicated thread pool 'publishOnScheduler(true)'
* try using client-side caching introduced in Redis 6 (compatible with lettuce)
* if you do not need strict consistency, implement a local cache with Reactor 'repository.findAll().cache(Duration.ofMillis(500))'
