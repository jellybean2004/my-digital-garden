---
{"dg-publish":true,"permalink":"/content/013/b-python/b7-type-hints/","noteIcon":"1","created":"2025-08-20T15:12:08.039+01:00","updated":"2025-08-20T15:45:11.772+01:00"}
---

- python is not a '**strongly typed**' language
- one does not have to explicitly state the variable type
- `mypy` program helps test the variable types

```python
number: int = int(input('number: '))
word: str = input('word: ')
```

- it can also be used to annotate functions

```python
def func(n: float) -> None:
	...

def func2(a: str, b: str) -> str:
	return a + b


```

## type aliases

```python
type Vector = list[float]

def scale(scalar: float, vector: Vector) -> Vector:
	return [scalar * num for num in vector]
```

- here, `Vector` instance is created
- to make it more explicit that this is a **type alias**, not a normal variable assignment:

```python
from typing import TypeAlias

Vector: TypeAlias = list[float]
```

## new type

```python
from typing import NewType

Id  = NewType(Id, int)
random_id = Id(1321)
random_id2 = Id(1354)

output = random_id + random_id2
# the type will be int
```

- the static type checker treats the new type as a subclass of the original type
- `int` operations can still be performed on `Id` but the result will be `int`



