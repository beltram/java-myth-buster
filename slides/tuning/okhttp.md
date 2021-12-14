## OkHttp tuning

* use [kotlinx.serialization converter](https://github.com/JakeWharton/retrofit2-kotlinx-serialization-converter)
* reuse connections 'ConnectionPool(100, 300, SECONDS)'
* configure maxRequests && maxRequestsPerHost
* use a service mesh for round-robin client-side load balancing (avoid sticky connections)