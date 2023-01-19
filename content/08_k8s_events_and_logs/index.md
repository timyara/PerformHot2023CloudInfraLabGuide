## Logs and Events

### K8s Events:
- K8s Events can be used to determine the health and status of critical components in your environment
- Events will be visible on all k8s entities in Dynatrace 
- Ensure k8s events are captured by enabling them in the settings section of your cluster
### K8s Logs:
- K8s System Logs are ingested from Nodes while Application logs are ingested from pods
- Logs will be visible on all k8s entities in Dynatrace 
- Log storage is enabled in global settings
- Logs ingestion is enabled at the host level
### Alerts & Metrics:
- You can create alerts and metrics from k8s events and logs by using the log viewer
