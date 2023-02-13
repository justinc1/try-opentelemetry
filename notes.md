## Links

- https://opentelemetry.io/
- https://www.codemag.com/Article/2301061/An-Introduction-to-Distributed-Tracing-with-OpenTelemetry-in-.NET-7

## Demo

- https://github.com/open-telemetry/opentelemetry-demo
  - http://localhost:8080/jaeger/ui/dependencies

- # https://opentelemetry.io/docs/collector/getting-started/
  - # http://localhost:9090 prometeus

## Loki

- https://grafana.com/docs/loki/latest/getting-started/
- https://grafana.com/docs/loki/latest/configuration/examples/
- https://grafana.com/blog/2022/06/23/how-to-send-logs-to-grafana-loki-with-the-opentelemetry-collector-using-fluent-forward-and-filelog-receivers/


```
docker rm -f loki
docker run -d --name=loki -p 3100:3100 --mount type=bind,source="$PWD/loki-config.yaml",target=/etc/loki/local-config.yaml grafana/loki

```
