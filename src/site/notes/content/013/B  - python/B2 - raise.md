---
{"dg-publish":true,"permalink":"/content/013/b-python/b2-raise/","noteIcon":"1","created":"2025-08-27T13:15:28.338+01:00","updated":"2025-08-20T15:49:47.000+01:00"}
---

```python
class Student:
    def __init__(self, name, house):
        if not name:
            raise ValueError("Missing name")
        if house not in ["Gryffindor", "Hufflepuff", "Ravenclaw", "Slytherin"]:
            raise ValueError("Invalid house")
        self.name = name
        self.house = house
        
    def __str__(self):
        return f"{self.name} from {self.house}"

def get_student():
    name = input("Name: ")
    house = input("House: ")
    return Student(name, house)

student = get_student()
print(student)
```

- this ensure that the the proper values are assigned to each attribute

- classes can also have built-in functions, called **methods**
- the ``__str__`` method provides a means by which a student is returned when called to be printed
- similarly, custom methods an be created
