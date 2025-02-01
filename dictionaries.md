# Dictionaries Methods and Properties Cheat Sheet

Python's **dictionary** is a powerful data structure that stores key-value pairs. It is implemented as a hash table, making it highly efficient for lookups, updates, and deletions. Here are the most commonly used **methods** and **properties** of dictionaries, along with examples.

---

## 🛠 Dictionary Methods

| **Method**             | **Description**                                                                 | **Example**                                  |
|-------------------------|---------------------------------------------------------------------------------|----------------------------------------------|
| `clear()`               | Removes all items from the dictionary.                                          | `d.clear()`                                  |
| `copy()`                | Returns a shallow copy of the dictionary.                                       | `new_dict = d.copy()`                        |
| `fromkeys(keys, value)` | Creates a dictionary from a sequence of keys and a single value.                | `d = dict.fromkeys(['a', 'b'], 0)`           |
| `get(key, default)`     | Returns the value for the key if it exists; otherwise, returns the default value.| `d.get('a', 'default')`                      |
| `items()`               | Returns a view object of key-value pairs.                                       | `for k, v in d.items(): print(k, v)`         |
| `keys()`                | Returns a view object of dictionary keys.                                       | `for key in d.keys(): print(key)`            |
| `pop(key, default)`     | Removes the specified key and returns its value.                                | `d.pop('a', 'default')`                      |
| `popitem()`             | Removes and returns the last inserted key-value pair as a tuple.                | `key, value = d.popitem()`                   |
| `setdefault(key, value)`| Returns the value for the key if it exists; otherwise, sets it to the default.   | `d.setdefault('a', 0)`                       |
| `update(other_dict)`    | Updates the dictionary with key-value pairs from another dictionary or iterable.| `d.update({'b': 2})`                         |
| `values()`              | Returns a view object of all dictionary values.                                 | `for value in d.values(): print(value)`      |

---

## 🗌 Dictionary Properties

| **Property**     | **Description**                                                                   | **Example**                      |
|-------------------|-----------------------------------------------------------------------------------|----------------------------------|
| Mutable           | Dictionaries can be modified after creation.                                     | `d['key'] = 'value'`             |
| Unordered         | Items are not stored in a specific order (Python 3.7+ maintains insertion order).| `d = {'b': 2, 'a': 1}`           |
| Keys Must Be Unique | Each key in a dictionary must be unique.                                          | `d = {'a': 1, 'a': 2}` (Keeps last value) |
| Keys Must Be Hashable | Keys must be immutable (e.g., strings, numbers, tuples).                         | `d = {(1, 2): 'value'}`          |

---

## 💡 Examples

### Example 1: Accessing and Updating Values
```python
d = {'a': 1, 'b': 2}
print(d['a'])    # Output: 1
d['c'] = 3        # Adds a new key-value pair
print(d)         # Output: {'a': 1, 'b': 2, 'c': 3}
```

### Example 2: Using `clear()`
```python
d = {'x': 10, 'y': 20}
d.clear()
print(d)  # Output: {}
```

### Example 3: Using `copy()`
```python
d = {'name': 'Alice'}
copy_d = d.copy()
copy_d['name'] = 'Bob'
print(d)       # Output: {'name': 'Alice'}
print(copy_d)  # Output: {'name': 'Bob'}
```

### Example 4: Using `fromkeys()`
```python
keys = ['name', 'age']
d = dict.fromkeys(keys, 'N/A')
print(d)  # Output: {'name': 'N/A', 'age': 'N/A'}
```

### Example 5: Using `get()`
```python
d = {'a': 1}
print(d.get('b', 0))  # Output: 0
```

### Example 6: Using `items()`
```python
d = {'name': 'Alice', 'age': 30}
for key, value in d.items():
    print(key, value)
# Output:
# name Alice
# age 30
```

### Example 7: Using `keys()`
```python
d = {'x': 10, 'y': 20}
print(list(d.keys()))  # Output: ['x', 'y']
```

### Example 8: Using `pop()`
```python
d = {'a': 1, 'b': 2}
removed_value = d.pop('a', 'not found')
print(removed_value)  # Output: 1
print(d)              # Output: {'b': 2}
```

### Example 9: Using `popitem()`
```python
d = {'a': 1, 'b': 2}
key, value = d.popitem()
print(key, value)  # Output: ('b', 2)
print(d)           # Output: {'a': 1}
```

### Example 10: Using `setdefault()`
```python
d = {'a': 1}
d.setdefault('b', 2)
print(d)  # Output: {'a': 1, 'b': 2}
```

### Example 11: Using `update()`
```python
d = {'a': 1}
d.update({'b': 2, 'c': 3})
print(d)  # Output: {'a': 1, 'b': 2, 'c': 3}
```

### Example 12: Using `values()`
```python
d = {'a': 1, 'b': 2}
print(list(d.values()))  # Output: [1, 2]
```

---

Continue exploring this repository for other data structures and their methods. 🚀


