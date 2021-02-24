# Convert unix timestamp to python datetime

Example on how to convert timestamp to datetime (from datetime library) using python

```python
from datetime import datetime

timestamp = 1545730073
dt_object = datetime.fromtimestamp(timestamp)

print("dt_object =", dt_object)
print("type(dt_object) =", type(dt_object))
```

For more info see the [docs](https://docs.python.org/3/library/datetime.html)
