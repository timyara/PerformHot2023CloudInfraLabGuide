## Create Static Threshold Alert

While Dynatrace will automatically detect when disk space is low, a few of our app teams are noisy loggers and we want to warn them of disk space utilization earlier.
We don’t want to change the OOTB Anomaly Detection as that will let us know when disk is critical. We just want an early warning alert.

![staticthreshold](../../assets/images/staticthreshold.png)

### Exercise Steps

1. Navigate to Settings > Anomaly Detection > Metric Events
2. Add a Metric Event
* Name: Disk Warning
* Type: Metric Key
* Metric Key: Disk Used %
* Aggregation: Average*
* Model Type: Static Threshold
* Threshold: 80%
* Alert Condition: Alert if metric is above
* Preview the alert with last 1, 3, and 7 days worth of data
* Title: Disk Warning
* Event Type: Custom Alert
* Do not allow to merge
