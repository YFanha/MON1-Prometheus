# Prometheus
Prometheus monitoring system deployment with Grafana.

## nginx_rproxy_config
Nginx virtual host to listen on 8080 and redirect to grafana (on root prefix) or to the prometheus web interface (/prometheus).

## prometheus.service.template
Template of the prometheus.service. The template already include de modification to work with the Nginx reverse proxy.
