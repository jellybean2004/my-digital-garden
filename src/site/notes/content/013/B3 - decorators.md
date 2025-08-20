---
{"dg-publish":true,"permalink":"/content/013/b3-decorators/","noteIcon":"1","created":"2025-08-20T10:35:18.238+01:00","updated":"2025-08-20T10:45:01.957+01:00"}
---

```python
class Student:
    def __init__(self, name, house):
        if not name:
            raise ValueError("Invalid name")
        self.name = name
        self.house = house

    def __str__(self):
        return f"{self.name} from {self.house}"

    # getter for house
    @property
    def house(self):
        return self._house

    # setter for house
    @house.setter
    def house(self, house):
        if house not in ["Gryffindor", "Hufflepuff", "Ravenclaw", "Slytherin"]:
            raise ValueError("Invalid house")
        self._house = house
```

- **decorators** are properties used to 'harden' the code
- here `@property` defined `_house` as a property of the class, allowing how `house` should be set and retrieved - **getter**
- the leading underscore indicates that the value need not be modified directly
- the **setter** is called whenever the house property is set to validate the input

