# Prometheus - basic

Run the prometheus server using the following command:

```
docker run -i --rm -p 9090:9090 \
    --volume=/Users/pyk/pyk/prometheus-samples:/etc \
    prom/prometheus:v2.1.0 \
    --config.file=/etc/prometheus.yaml
```

Access [localhost:9090](http://localhost:9090) for prometheus dashboard.

Run grafana:

```
docker run -i --rm -p 3000:3000 grafana/grafana:4.6.3
```

Access [localhost:3000] to access grafana dashboard.
