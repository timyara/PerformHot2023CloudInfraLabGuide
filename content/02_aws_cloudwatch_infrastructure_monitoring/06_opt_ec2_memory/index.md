## (Optional) EC2 Memory


Chart the memory consumed by your EC2 instances​

![02_06_ec2memory](../../../assets/images/02_06_ec2memory.png)


1. Select on the left Menu "Data explorer"​
2. On the top right corner, select the chart as "Graph"​
3. On the metric selection type "builtin:host.mem.usage"​
4. Leave aggregation as Auto(avg)​
5. Split by "Host"​
6. Filter by "Host" > "Cloud Type" > "EC2"​
7. Click on "Run query" button​
8. On the right menu​
9. In "Axes" section, edit the "Left" "Min, Max" to 0, 100​
10. In Threshold section,  yellow ≥ 70, red ≥ 90  (leave green without any value)​
11. Click on "Pin to Dashboard" button and add it to your dashboard "AWS overview"​
