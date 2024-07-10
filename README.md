# My custom Grafana resources

## Dashboards

### K8s
- <b>k8s/k8s-custom-metrics.json</b> <br>
My own dashboard to explore Kubernetes resources. It uses 
metrics from Prometheus and kube-stat-metrics as metircs exporter. It also has panel to watch logs of container via Loki datasource.

### Yandex.Cloud
If you don't want to use Yandex Monitoring to monitor your cloud resources you can configure cloud to share metrics with your own Prometheus instance: https://yandex.cloud/en/docs/monitoring/operations/metric/prometheusExport
- <b>yandex_cloud/yandex-certificates.json</b> <br>
Dashboard to explore Certificate Manager. It has two panels: certificates' expiriation and out of order certificates. So you can create alerts based on these panels.

- <b>yandex_cloud/yandex-compute.json</b> <br>
Dashboard to explore Compute Cloud. It shows information about CPU, Disk and Network. I don't recommend to use metrics from Yandex Monitoring to check VM status. Instead of that you can configure basic Node Exporter, it provides more information!

- <b>yandex_cloud/yandex-kafka.json</b> <br>
Dashboard to check Kafka's metrics. It has very large collection of panels. You can see there brokers' status, topics' and whole cluster size, CPU/Memory usage, etc. 

- <b>yandex_cloud/yandex-postgres.json</b> <br>
Dashboard to explore PostgreSQL cluster. It gives information about running status, compute resource usage, information about connections, transactions, sessions and databases list.  
