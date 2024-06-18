 # Prometheus
Deployment of a Prometheus monitoring system with Grafana.

# Files
These files are updated with the progress of the project

## Templates

### Templates/grafana_RProxy.template
Nginx virtual host to listen on 8080 and redirect to the wanted services.
- / -> grafana (port 3000)
- /prometheus/ -> prometheus web interface (port 9090)

### Templates/prometheus.service.template
Template of the prometheus.service. The template already include the modifications to work with the Nginx reverse proxy.

## Configuration-AWS
Store the actuals configuration files of the prometheus's components. 
- Prometheus (/app/prometheus2.51.2)
- Alertmanager (/app/alertmanager.yml/)
- service_restarter (/etc/service_restarter)
- prometheus.service (/etc/systemd/system/prometheus.service)
- alertmanager.service (/etc/systemd/system/alertmanager.service)
- service_restarter.service (/etc/systemd/system/service_restarter.service)
