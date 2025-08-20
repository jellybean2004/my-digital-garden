---
{"dg-publish":true,"permalink":"/content/013/b1-introduction/","noteIcon":"1","created":"2025-08-20T09:55:52.970+01:00","updated":"2025-08-20T10:16:18.682+01:00"}
---

## classes
- a mould for data where data types can be defined and named

```python
class Student:
	def __init__(self, name, house):
		self.name = name
		self.house = house

def main():
    student = get_student()
    print(f"{student.name} from {student.house}")

def get_student():
    student.name = input("Name: ")
    student.house = input("House: ")
    return Student

if __name__ == "__main__":
    main()
```

- **convention:** class names are capitalised
- here, **student** is an **object**