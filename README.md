# Integrating Alfresco Transform Service with Prometheus

This project includes a Docker Compose template to provide a sample configuration that connects Alfresco Transform Service metrics endpoint with Prometheus.

* [.env](.env) specifies Alfresco Services version to be used by Docker Compose
* [compose.yaml](compose.yaml) describes Docker Compose deployment
* [prometheus.yml](prometheus.yml) includes sample Prometheus configuration for `transform-router` and `transform-core-aio` services

>> Note this is a sample deployment designed for education purposes. When using Alfresco Transform Service in real world, additional requirements should impact in the design of the final deployment.

## Using

```
docker-compose up --build --force-recreate
```

## Service URLs

* Prometheus: http://localhost:9090
* Transform Router Metrics: http://localhost:8095/actuator/prometheus
* Transform Core AIO Metrics: http://localhost:8090/actuator/prometheus