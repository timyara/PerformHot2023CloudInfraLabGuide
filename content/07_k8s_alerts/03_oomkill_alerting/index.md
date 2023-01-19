## OOM Alert

### Configure a custom alert for OOM Kills on containers

1. Navigate to Settings > Anomaly detection > Metric events
2. Click the **Add metric event** button
3. Configure the new metric event with the following details
- Summary: *Container OOMKills High*
- Type: *Metric key*
- Metric key: *Kubernetes: Container - out of memory (OOM) kill count*
- Static Threshold: *1*
- Event title: *Container OOMKills high for {entityname}*
4. Click the **Save** changes button

