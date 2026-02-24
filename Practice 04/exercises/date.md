# Python Date

## 1. Subtract 5 days
This program gets the current date and subtracts 5 days using timedelta.

```python
from datetime import datetime, timedelta

now = datetime.now()
print(now - timedelta(days=5))
```

## 2. Yesterday, Today, Tomorrow
This program prints yesterday, today and tomorrow.

```python
from datetime import date, timedelta

today = date.today()
print(today - timedelta(days=1))
print(today)
print(today + timedelta(days=1))
```

## 3. Drop microseconds
This removes microseconds from current time.

```python
from datetime import datetime

dt = datetime.now()
print(dt.replace(microsecond=0))
```

## 4. Difference in seconds
This calculates difference between two dates in seconds.

```python
from datetime import datetime

d1 = datetime(2024, 1, 1)
d2 = datetime(2024, 1, 10)

print((d2 - d1).total_seconds())
```

print((d2 - d1).total_seconds())
```
