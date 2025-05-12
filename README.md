# Python Data Types 🐍

A comprehensive guide to Python's built-in data types, with examples, comparisons, and best practices. Ideal for beginners and a quick reference for experienced developers.

## 📋 Table of Contents
- [Built-in Data Types](#built-in-data-types)
- [Type Conversion](#type-conversion)
- [Mutability vs Immutability](#mutability-vs-immutability)
- [Type Checking](#type-checking)
- [Advanced Typing (Type Hints)](#advanced-typing-type-hints)
- [Resources](#resources)

---

## Built-in Data Types
Python has several built-in data types, categorized as:

### 🔢 Numeric Types
- `int`: Integer (e.g., `5`, `-3`, `0`)
- `float`: Floating-point number (e.g., `3.14`, `-0.001`)
- `complex`: Complex number (e.g., `1 + 2j`)

### ✨ Sequence Types
- `str`: Immutable string (e.g., `"hello"`, `'Python'`)
- `list`: Mutable ordered sequence (e.g., `[1, 2, 3]`)
- `tuple`: Immutable ordered sequence (e.g., `(1, 2, 3)`)

### 🗃️ Mapping Type
- `dict`: Key-value pairs (e.g., `{"name": "Alice", "age": 25}`)

### ⚡ Set Types
- `set`: Unordered, mutable, unique elements (e.g., `{1, 2, 3}`)
- `frozenset`: Unordered, immutable version of `set`

### ❓ Boolean Type
- `bool`: `True` or `False`

### 🗑️ None Type
- `None`: Represents absence of value.

---

## Type Conversion
Convert between types using built-in functions:
```python
num_str = "123"
num_int = int(num_str)  # Convert string to int
num_float = float(num_str)  # Convert string to float
str_num = str(123)  # Convert int to string
Mutability vs Immutability
Mutable: Can be changed after creation (list, dict, set).

python
my_list = [1, 2, 3]
my_list[0] = 99  # Valid
Immutable: Cannot be changed after creation (int, float, str, tuple, frozenset).

python
my_tuple = (1, 2, 3)
my_tuple[0] = 99  # TypeError!
Type Checking
Check a variable's type using type() or isinstance():

python
x = 3.14
print(type(x))         # <class 'float'>
print(isinstance(x, float))  # True
Advanced Typing (Type Hints)
Python supports type annotations for clarity and static checking (PEP 484):

python
def greet(name: str) -> str:
    return f"Hello, {name}"

# Static type checkers (e.g., mypy) will validate types.
Resources
Python Docs: Built-in Types

Real Python: Data Types Guide

Typing Module (PEP 484)
