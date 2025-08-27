---
{"dg-publish":true,"permalink":"/content/013/b-python/b4-methods/","noteIcon":"1","created":"2025-08-27T13:15:28.347+01:00","updated":"2025-08-20T10:54:14.000+01:00"}
---

```python
import random

class Hat:

    houses = ["Gryffindor", "Hufflepuff", "Ravenclaw", "Slytherin"]

    @classmethod
    def sort(cls, name):
        print(name, "is in", random.choice(cls.houses))

Hat.sort("Harry")
```

- the `sort` method prints the student's assigned house
- as `__init__` is removed, since it need no be instantiated, `cls` replaces `self`
