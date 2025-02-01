# Strings Methods and Properties Cheat Sheet

Python's **string** is an immutable sequence of characters, widely used for text manipulation. Strings in Python come with a rich set of **methods** and **properties** for working with text effectively.

---

## 🛠 String Methods
Here are the most commonly used string methods:

| **Method**              | **Description**                                                                                 | **Example**                       |
|--------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------|
| `capitalize()`           | Converts the first character of the string to uppercase.                                        | `'hello'.capitalize()` → `'Hello'` |
| `lower()`                | Converts all characters to lowercase.                                                          | `'HELLO'.lower()` → `'hello'`     |
| `upper()`                | Converts all characters to uppercase.                                                          | `'hello'.upper()` → `'HELLO'`     |
| `title()`                | Converts the first character of each word to uppercase.                                        | `'hello world'.title()` → `'Hello World'` |
| `strip()`                | Removes leading and trailing whitespace (or specified characters).                             | `' hello '.strip()` → `'hello'`   |
| `replace(old, new)`      | Replaces occurrences of a substring with another substring.                                     | `'hello'.replace('l', 'x')` → `'hexxo'` |
| `split(sep)`             | Splits the string into a list based on the specified separator.                                 | `'a,b,c'.split(',')` → `['a', 'b', 'c']` |
| `join(iterable)`         | Joins elements of an iterable with the string as the separator.                                 | `','.join(['a', 'b', 'c'])` → `'a,b,c'` |
| `startswith(prefix)`     | Checks if the string starts with the specified prefix.                                         | `'hello'.startswith('he')` → `True` |
| `endswith(suffix)`       | Checks if the string ends with the specified suffix.                                           | `'hello'.endswith('lo')` → `True` |
| `find(sub)`              | Returns the index of the first occurrence of the substring (or `-1` if not found).             | `'hello'.find('l')` → `2`         |
| `count(sub)`             | Returns the number of occurrences of a substring in the string.                                | `'hello'.count('l')` → `2`        |
| `isdigit()`              | Checks if all characters in the string are digits.                                             | `'123'.isdigit()` → `True`        |
| `isalpha()`              | Checks if all characters in the string are alphabetic.                                         | `'abc'.isalpha()` → `True`        |
| `isalnum()`              | Checks if all characters in the string are alphanumeric.                                       | `'abc123'.isalnum()` → `True`     |
| `len()`                  | Returns the length of the string.                                                              | `len('hello')` → `5`              |

---

## 🗌 String Properties

| **Property**       | **Description**                                                               | **Example**                   |
|---------------------|-------------------------------------------------------------------------------|-------------------------------|
| Immutable          | Strings cannot be modified after creation.                                    | `s = 'hello'`                 |
| Ordered            | Strings maintain the order of characters.                                     | `s = 'world'`                 |
| Indexable          | Characters in a string can be accessed using their index.                    | `s[0]` → `'w'`                |
| Iterable           | Strings can be iterated over in a loop.                                       | `for c in 'abc': print(c)`    |

---

## 💡 Examples

### Example 1: Basic String Operations
```python
s = "hello world"
print(s.capitalize())  # Output: "Hello world"
print(s.upper())       # Output: "HELLO WORLD"
print(s.split())       # Output: ["hello", "world"]
```

### Example 2: String Indexing and Iteration
```python
s = "python"
print(s[0])            # Output: 'p'
for c in s:
    print(c)          # Outputs each character
```

### Example 3: Immutability
```python
s = "immutable"
# s[0] = "I"  # Raises TypeError because strings are immutable.
```

### Example 4: Joining and Splitting
```python
txt = "a,b,c"
parts = txt.split(",")
print(parts)          # Output: ["a", "b", "c"]
joined = "-".join(parts)
print(joined)         # Output: "a-b-c"
```

### Example 5: Using `startswith()` and `replace()`
```python
text = "python programming"
print(text.startswith("python"))  # Output: True
print(text.replace("python", "Java"))  # Output: "Java programming"
```

### Example 6: Checking String Properties with `isalnum()` and `isdigit()`
```python
code = "abc123"
print(code.isalnum())  # Output: True
num_str = "12345"
print(num_str.isdigit())  # Output: True
```


Strings are fundamental in Python, and mastering their methods and properties will make your code cleaner and more efficient. 🚀
