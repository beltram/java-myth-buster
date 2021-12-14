## Redis

* activate connection keep-alive (not by default) 'socketOptions(SocketOptions.builder().keepAlive(true).build())'
* offload cpu intensive operations to a dedicated thread pool 'publishOnScheduler(true)'
* try using client-side caching introduced in Redis 6 (compatible with lettuce)
