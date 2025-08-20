---
{"dg-publish":true,"permalink":"/content/013/b6-operator-overloading/","noteIcon":"1","created":"2025-08-20T11:00:43.606+01:00","updated":"2025-08-20T11:03:46.556+01:00"}
---

```python
class Vault:
    def __init__(self, galleons=0, sickles=0, knuts=0):
        self.galleons = galleons
        self.sickles = sickles
        self.knuts = knuts

    def __str__(self):
        return f"{self.galleons} Galleons, {self.sickles} Sickles, {self.knuts} Knuts"

    def __add__(self, other):
        galleons = self.galleons + other.galleons
        sickles = self.sickles + other.sickles
        knuts = self.knuts + other.knuts
        return Vault(galleons, sickles, knuts)


potter = Vault(100, 50, 25)
print(potter)

weasley = Vault(25, 50, 100)
print(weasley)

total = potter + weasley
print(total)
```

- operators such as `+` and `-` can be 'overloaded' to perform more than just simple arithmetic
- here, `__add__` adds the values of two vaults
