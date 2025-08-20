---
{"dg-publish":true,"permalink":"/content/013/b-python/b5-inheritance/","noteIcon":"1","created":"2025-08-20T10:54:31.893+01:00","updated":"2025-08-20T10:59:40.343+01:00"}
---

```python
class Wizard:
    def __init__(self, name):
        if not name:
            raise ValueError("Missing name")
        self.name = name

    ...


class Student(Wizard):
    def __init__(self, name, house):
        super().__init__(name)
        self.house = house

    ...


class Professor(Wizard):
    def __init__(self, name, subject):
        super().__init__(name)
        self.subject = subject

    ...


wizard = Wizard("Albus")
student = Student("Harry", "Gryffindor")
professor = Professor("Severus", "Defense Against the Dark Arts")
...
```

- another class that **'inherits'** methods, variables and attributes from a class can be created
- here, both `Student` and `Professor` inherit the characteristics of `Wizard` as both are wizards
- so `Student` is a **'child'** class, while `Wizard` is a **'parent'** or **'super'** class
- `super().__init__(name)` runts the `init` method of `Wizard`

