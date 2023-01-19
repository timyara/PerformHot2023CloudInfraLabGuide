## Log Metric Alert

- My AWS networking team wants to alert on the CLB request processing time, but doesn’t know what they should use for the threshold.

![logmetricalert](../../../assets/images/logmetricalert.png)

### Exercise Steps
- Find the RDS connect error log records
- Navigate to  Settings> Anomaly Detection> Metric Events
- Add metric event
- Summary: CLB Request Processing Time
- Metric Selector: log.clb.requestprocessingtime
- Aggregation: Average
- Model type: Auto-adaptive threshold
- Do not alert on missing data (best practice for log metrics)
- Alerting Condition Alert if metric is above
- Title: CLB Request Processing Time
- Event Type: Slowdown
- Allow to merge
- Save Changes
