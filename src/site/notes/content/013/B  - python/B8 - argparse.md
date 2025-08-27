---
{"dg-publish":true,"permalink":"/content/013/b-python/b8-argparse/","noteIcon":"1","created":"2025-08-27T13:15:28.362+01:00","updated":"2025-08-21T09:26:23.000+01:00"}
---

```python
import argparse

parser = argparse.ArgumentParser(description="Meow like a cat")
parser.add_argument("-n", default=1, help="number of times to meow", type=int)
args = parser.parse_args()

for _ in range(args.n):
    print("meow")
```

- `argparse` library handles the parsing of complicated strings from command-line arguments
- `parser` is an object from an `ArgumentParser` class
- `add_argument` method tells what arguments should be expected when the user runs the program
- `parse_args` method ensures that all the arguments have been included by the user
- the bracketed terms provide user with more documentation
