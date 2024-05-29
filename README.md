# Prometheus
Prometheus monitoring system deployment with Grafana.

# Files
These files are updated with the progress of the project

## nginx_rproxy_config
Nginx virtual host to listen on 8080 and redirect to the wanted services.
- / -> grafana (port 3000)
- /prometheus/ -> prometheus web interface (port 9090)

## prometheus.service.template
Template of the prometheus.service. The template already include the modifications to work with the Nginx reverse proxy.
