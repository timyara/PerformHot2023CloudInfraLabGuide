## Unused provisioned volumes

Identify if you have EBS volumes allocated but with very low utilization
By monitor this metric you can verify that provisioned resources are not going unused. Sudden spikes in idle time could indicate issues in your application, preventing it from sending requests the provisioned volumes.​

![02_05_ebsidle](../../../assets/images/02_05_ebsidle.png)

1. Select on the left Menu "Data explorer"​
2. On the top right corner, select the chart as "Graph"​

![02_05_chartselector](../../../assets/images/02_05_chartselector.png)
3. On the metric selection type "EBS volume idle time %"​
4. Leave aggregation as Auto(avg)​
5. Split by "EBS volume"​
6. Click on "Run query" button​
7. Click on "Pin to Dashboard" button and add it to your dashboard "AWS overview"
