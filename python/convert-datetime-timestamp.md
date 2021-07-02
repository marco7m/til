# Convert python datetime to unix timestamp

Simple example of an **aware** (with tzinfo setted to local time zone) datetime variable (from datetime library) converted to unix timestamp:

```python
from datetime import datetime

now = datetime.now()

# convert
timestamp = now.timestamp()
print("timestamp =", timestamp)
```

When reading a datetime value from SQL with python, its value will be stored as a **naive** (with tzinfo = None) datetime python variable (from datetime library). The *timestamp()* method of the *datetime* object always consider a **naive** datetime as if it is in the local time zone, if the *datetime* should be in UTC 0 time zone whe must replace its time zone when getting the timestamp. The example below show how to convert it to unix timestamp:

```python
from datetime import datetime
import pymysql

# Read a datetime from pymysql and store it as my_datetime

# convert
timestamp = my_datetime.replace(tzinfo=timezone.utc).timestamp()
print("timestamp =", timestamp)
```


For more info see the [docs](https://docs.python.org/3/library/datetime.html)
