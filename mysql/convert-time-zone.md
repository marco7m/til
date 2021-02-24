To convert a DATETIME in MySQL to a different time zone the following command can be used:

```sql
CONVERT_TZ (dt, from_tz,to_tz)
```

The example below prints the current time in Brasilia local time.
```sql
SELECT CONVERT_TZ(NOW(),'+00:00','-03:00');
```
