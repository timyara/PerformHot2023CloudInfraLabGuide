## Charting Logs

### Exercise Steps

1. Navigate to the Logs & Events Viewer​
2. Filter by event.type: log
```bash
event.type: log
```
3. Click into an log entry to see what attributes are captured​
4. Add a filter for our namespace
```bash
k8s.namespace.name: NAMESPACE_NAME
```
5. Add a filter for our container
```bash
k8s.container.name: CONTAINER_NAME
```
6. Filter the content for "update"​
```bash
content: update
```
7. Format the table by adding the fields below:​
* dt.source_entity​
* k8s.container.name​
* k8s.namespace.name
* dt.kubernetes.cluster.name​

8. Pin the table to your dashboard

![charted_logs](../../../assets/images/k8slogs4.jpg)
