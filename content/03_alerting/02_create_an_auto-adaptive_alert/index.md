## Create an Auto-Adaptive Alert

- We sometimes get 4xx errors on the ALB and have accepted that we can’t fix 100% of errors.
- However, we want to Dynatrace to tell us if errors spike up outside of the norm without having to create thresholds ourselves.
- The number of errors may fluctuate, and it would be great if Dynatrace could auto-adapt and let us know when big spikes occur


![autoadaptive](../../assets/images/autoadaptive.png)

### Exercise Steps

1. Navigate to Settings > Anomaly Detection > Metric Events
2. Add a Metric Event
* Name: ALB Errors
* Type: Metric Selector
* Metric Selector: builtin:cloud.aws.alb.errors.alb.http4xx 
* Model Type: Auto-Adaptive Threshold
* Don’t alert on missing data
* Alert Condition: Alert if metric is above
* Preview the alert with last 1, 3, and 7 days' worth of data
* Title: ALB Errors
* Event Type: Error
* Allow to merge
