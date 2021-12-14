## R2DBC

* now faster than jpa
* use connection pooling
  * requires r2dbc-pool on the classpath
  * increase 'spring.r2dbc.pool.max-size' (defaults to 10)
  * watch PostgreSQL connection limit (1500 for RDS)
