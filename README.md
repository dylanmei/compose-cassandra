compose-cassandra
-----------------

Spin up a Cassandra cluster based on the [library/cassandra](https://hub.docker.com/_/cassandra/) image.

```
docker-compose up
docker run -it --link composecassandra_cassandra0_1:cassandra --rm cassandra:2.2.3 sh -c 'exec cqlsh "$CASSANDRA_PORT_9042_TCP_ADDR"'
```

