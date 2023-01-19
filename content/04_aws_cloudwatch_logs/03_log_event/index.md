## Log Event

- I shouldn’t see any connection issues coming from my RDS instance, but it’s happened in the past
- When that happens, I want Dynatrace to create a log event and alert on it.


![logevent1](../../assets/images/logevent1.png)

### Find the RDS Log
- Find the RDS connect error log records
- Search content:

```bash
unable to connect
```
- Copy the entire log content

![logevent2](../../assets/images/logevent2.png)

### Create Log Event
- Navigate to Settings> Log Monitoring> Events Extraction
- Add log event
- Summary: RDS Connection Error
- Log Query:
```bash
content="error: 2 The following error occurred: Can't connect to MySQL server on 'db-qig94285-ac32d6-2a.rds.amazonaws.com' (10060) QMYSQL: Unable to connect”
```
- Title: RDS Connection Error
- Event Type: Error
- Allow to Merge
- Save Changes
