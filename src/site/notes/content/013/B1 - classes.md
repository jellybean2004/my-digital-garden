---
{"dg-publish":true,"permalink":"/content/013/b1-classes/","noteIcon":"1","created":"2025-08-20T09:55:52.970+01:00","updated":"2025-08-20T10:19:34.826+01:00"}
---

- a **class** is a mould for data where custom data types can be defined and named

```python
class Student:
	def __init__(self, name, house):
		self.name = name
		self.house = house

def get_student():
    name = input("Name: ")
    house = input("House: ")
    return Student(name, house)

student = get_student()
print(f"{student.name} from {student.house}")
```

- **convention:** class names are capitalised
- here, **student** is an **object**