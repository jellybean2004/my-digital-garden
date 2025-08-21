---
{"dg-publish":true,"permalink":"/content/013/b-python/b11-filter/","noteIcon":"1","created":"2025-08-21T09:44:36.528+01:00","updated":"2025-08-21T09:52:51.811+01:00"}
---

```python
students = [
    {"name": "Hermione", "house": "Gryffindor"},
    {"name": "Harry", "house": "Gryffindor"},
    {"name": "Ron", "house": "Gryffindor"},
    {"name": "Draco", "house": "Slytherin"},
]

def is_gryffindor(s):
    return s["house"] == "Gryffindor"

gryffindors = filter(is_gryffindor, students)

for gryffindor in sorted(gryffindors, key=lambda s: s["name"]):
    print(gryffindor["name"])
```

- `filter` takes two arguments
- the first is a function that returns `True` or `False`
- the second is the sequence which is to be filtered
- furthermore, a lambda function can be used to simplify it, removing the need to have a defined function

```python
gryffindors = filter(lambda s: s["house"] == "Gryffindor", students)
```

