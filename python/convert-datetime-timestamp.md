# Convert python datetime to unix timestamp

When reading a datetime value from SQL with python, its value will be stored as a datetime python variable (from datetime library). The example below show how to convert it to unix timestamp.

```python
from datetime import datetime

now = datetime.now()

# convert
timestamp = datetime.timestamp(now)
print("timestamp =", timestamp)
```
For more info see the [docs](https://docs.python.org/3/library/datetime.html)
