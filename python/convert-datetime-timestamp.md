# Convert python datetime to unix timestamp

```python
from datetime import datetime

now = datetime.now()

# convert
timestamp = datetime.timestamp(now)
print("timestamp =", timestamp)
```
