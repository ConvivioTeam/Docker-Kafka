# Apache Kafka Docker image

Based on [Kafka Docker image from wurstmeister](https://github.com/wurstmeister/kafka-docker).

Adds a [healthcheck for Docker compose](https://github.com/wurstmeister/kafka-docker/issues/167#issuecomment-439849789) from [Lukkie](https://github.com/Lukkie).

The healthcheck can be added to your Docker compose file like this:

```
    healthcheck:
      test: ["CMD-SHELL", "/bin/healthcheck.sh"]
      interval: 5s
      timeout: 10s
      retries: 5
```
