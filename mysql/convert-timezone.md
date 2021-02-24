To convert a DATETIME in MySQL to a different timezone the following command can be used:

```sql
CONVERT_TZ (dt, from_tz,to_tz)
```

The example below prints the current time in Brasilia timezone.
```sql
SELECT CONVERT_TZ(NOW(),'+00:00','-03:00');
```
