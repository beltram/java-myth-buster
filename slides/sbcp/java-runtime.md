## Java runtime

* Java 11
* Netty
* Spring Boot + Spring Webflux
* Reactive drivers for Redis, PostgreSQL, MongoDB, Kafka
* OkHttp + Retrofit
* Distributed concerns delegated to Kubernetes + Istio, apps does not handle: 
  * Circuit breaking (Hystrix, resilience4J)
  * Configuration server (Archaius, Spring Cloud Config)
  * Client side load balancing (Ribbon, Spring Cloud LoadBalancer)
  * Service registry (Eureka)
