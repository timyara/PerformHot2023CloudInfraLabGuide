## Set Alerts to Alerting Profile

- We want send a notification just to the app team with the noisy logging when the Disk Warning Triggers.
- We can group alerts based on severity, impact, and tags with alerting profiles.


![diskalert1](../../assets/images/diskalert1.png)

### Exercise Steps

1. Navigate to Settings > Alerting > Problem Alerting Profiles
2. Add a Metric Event for just the Disk Warning Alert
* Name: Disk Warning
* Problem Severity: Custom
* Problem Delay in Minutes: 10 minutes
* Filter problems by tag: Include All Entities
* Event Filter: Custom
* Title Filter: Equals Disk Warning
* Enabled
* Save Changes

![diskalert2](../../assets/images/diskalert2.png)
