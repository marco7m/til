# Convert unix timestamp to python datetime

Example on how to convert timestamp to datetime (from datetime library) using python

```python
from datetime import datetime

timestamp = 1545730073
dt_object = datetime.fromtimestamp(timestamp, tz=timezone.utc)

print("dt_object =", dt_object)
print("type(dt_object) =", type(dt_object))
```

Setting **tz=timezone.utc** is necessary to not change the time zone to the local time zone. When using this function without a tz, like this:

```python
datetime.fromtimestamp(timestamp, tz=None)  # Same as datetime.fromtimestamp(timestamp)
```

It will automatically convert to the local system time zone.

For more info see the [docs](https://docs.python.org/3/library/datetime.html)
