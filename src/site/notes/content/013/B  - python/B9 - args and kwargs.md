---
{"dg-publish":true,"permalink":"/content/013/b-python/b9-args-and-kwargs/","noteIcon":"1","created":"2025-08-21T09:27:48.812+01:00","updated":"2025-08-21T09:33:53.818+01:00"}
---

- `args` are positional arguments
- `kwargs` are named or '**keyword**' arguments

```python
print(*objects, sep=' ', end='\n', file=sys.stdout, flush=False)
```

- here, for `print`:
	- `args` would be `*objects`, which are things to print
	- `kwards` would be `end =  ""`

```python
def f(*args, **kwargs):
    print("Positional:", args)

# positional arguments
f(100, 50, 25)

# named/keyword arguments
f(galleons=100, sickles=50, knuts=25)
```
