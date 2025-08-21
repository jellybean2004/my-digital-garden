---
{"dg-publish":true,"permalink":"/content/013/b-python/b10-list-comprehension/","noteIcon":"1","created":"2025-08-21T09:37:53.986+01:00","updated":"2025-08-21T09:44:17.705+01:00"}
---

```python
def main():
    yell("This", "is", "CS50")

def yell(*words):
    uppercased = []
    for word in words:
        uppercased.append(word.upper())
    print(*uppercased)

if __name__ == "__main__":
    main()```

- using `map`, the above function can be simplified

```python
def yell(*words):
    uppercased = map(str.upper, words)
    print(*uppercased)
```

- using **list comprehension**, it can be turned into a one-liner

```python
uppercased = [arg.upper() for arg in words]
```

- similarly, for a dictionary:

```python
students = [
    {"name": "Hermione", "house": "Gryffindor"},
    {"name": "Harry", "house": "Gryffindor"},
    {"name": "Ron", "house": "Gryffindor"},
    {"name": "Draco", "house": "Slytherin"},
]

gryffindors = []
for student in students:
    if student["house"] == "Gryffindor":
        gryffindors.append(student["name"])

for gryffindor in sorted(gryffindors):
    print(gryffindor)
```

- list comprehension can simplify this

```python

griffindoes = [student for student in students if student["house"] == "Griffindor"]
```
