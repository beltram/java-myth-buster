## r2dbc

* now faster than jpa
* use connection pooling
  * requires r2dbc-pool on the classpath
  * spring.r2dbc.pool.max-size=50 (defaults to 10)
  * watch PostgreSQL connection limit (1500 for RDS)