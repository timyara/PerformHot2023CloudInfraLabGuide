## Monitor additional service metrics

The application team that uses AWS Kinesis Data streams wants to monitor additional metrics due to the high increase of utilization. They would like to know if the "IncomingRecords" are still under the initially scope range or higher.​

Add the metric "IncomingRecords" to the AWS Kinesis Data Streams



1. Access to Dynatrace UI​
2. Click on Setting, on the left Menu ​
3. Expand the "Cloud and virtualization" section​
4. Select AWS​
5. Edit (pencil icon) the current AWS connection​
6. Click on Manage Services​
7. Select the Service "AWS Kinesis Data Streams"​
8. Click on Add Metric​
9. Select the "IncommingRecords" metric ​
10. Select the statistics "Average + Minimum + Maximum"​
11. Select the dimension "StreamName"​
12. Add metric​

- Note: Don’t save it, as you don’t have the permissions to add it
