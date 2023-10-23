# Kubernetes monitoring

Here you can find monitoring systems for the docker monolith or kubernetes cluster. The monitoring package includes Prometheus, Node-exporter, AlertManager, BlackBox-Exporter.


### Docker compose:

- `alertmanager.yml` : slack_configs.api_url - your slack web hook url
- `prometheus.yml` : job_name - 'blackbox' -> targets: your thingsboard domain



- to deploy monitoring systems, run the script `./docker-monitoring-deploy.sh`;

- to delete monitoring systems run the script `./docker-delete-monitoring.sh`;


### Kubernetes

 - `alertmanager/alert-configMap.yml` : slack_configs.api_url - your slack web hook url
 - `prometheus/prometheus-configMap.yml` : job_name - 'kube-api-blackbox -> targets: your thingsboard domain



- to deploy monitoring systems, run the script `./k8s-deploy-monitoring.sh`

- to delete monitoring systems run the script `./k8s-delete-monitoring.sh`
