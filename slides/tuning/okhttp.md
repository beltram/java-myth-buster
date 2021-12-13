## okhttp tuning

* use [kotlinx.serialization converter](https://github.com/JakeWharton/retrofit2-kotlinx-serialization-converter)
* reuse connections 'ConnectionPool(100, 300, SECONDS)'
* high max requests 'Dispatcher(Dispatcher().executorService).apply { maxRequests = 5000; maxRequestsPerHost = 5000 }'
* use a service mesh for round-robin client-side load balancing (avoid sticky connections)