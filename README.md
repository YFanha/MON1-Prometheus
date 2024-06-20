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

## Documentation
Images/Schema for the wiki.

## alertmanager
Files of the **running** Alertmanager instance (/app/alertmanager).

## prometheus2.51.2
Files of the **running** Prometheus instance (/app/prometheus2.51.2).

## alertnames.yml
> /etc/service_restarter.yml (Hard link) \
File for service_restarter.

## Services files

### alertmanager.service
> /etc/systemd/system/alertmanager.service (Hard link) \
Service file of Alertmanager. Store the alerts that should trigger a service restart.

### prometheus.service
> /etc/systemd/system/prometheus.service (Hard link) \
Service file of Prometheus.

### service_restarter.service
> /etc/systemd/system/service_restarter.service (Hard link) \
Service file of [Service Restarter](https://github.com/YFanha/service_restarter).
