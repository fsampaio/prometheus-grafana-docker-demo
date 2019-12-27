# Prometheus-Grafana Demo

Run [Prometheus](https://github.com/prometheus/prometheus), [Node Exporter](https://github.com/prometheus/node_exporter), and [Grafana](https://github.com/grafana/grafana) with a simple `docker-compose.yml` file.

## Setup

```bash
git clone https://github.com/mewil/prometheus-grafana-docker-demo
cd prometheus-grafana-docker-demo
docker-compose up -d
```

Open http://localhost:3000/ in your browser to see Grafana. From there, you can add a data source for Prometheus, with the URL `http://prometheus:9090`, and head to the explore tab to see the metrics coming in.

To view Prometheus go to http://localhost:9090/ and to view the exporter go to http://localhost:9100/.

To view the logs, run `docker-compose logs -f` and to stop and remove the containers, run `docker-compose down`.
