Monitoring system for endpoints, run it with docker-compose.

Containers:
1) proxy - nginx web server for monitoring UI tools (nginx.conf config, certs for Your site in 'ssl' directory)
2) prometheus - monitoring system & time series database inside the container (prometheus.yml config)
3) blackbox_exporter - Prometheus module for checking endpoints (HTTP, HTTPS, DNS, TCP, ICMP) (blackbox.yml config)
4) grafana - visualisation and alerting system based on official container image
5) node-exporter - monitoring for server itself
