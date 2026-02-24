# Python Generators

## Squares up to N
This generator returns square numbers up to N.

```python
def squares(n):
    for i in range(1, n + 1):
        yield i * i

for x in squares(5):
    print(x)
```

## Even numbers
This generator returns even numbers from 0 to N.

```python
def evens(n):
    for i in range(n + 1):
        if i % 2 == 0:
            yield i

print(",".join(map(str, evens(20))))
```

## Divisible by 3 and 4
This generator returns numbers divisible by 3 and 4.

```python
def div(n):
    for i in range(n + 1):
        if i % 3 == 0 and i % 4 == 0:
            yield i

print(list(div(50)))
```
