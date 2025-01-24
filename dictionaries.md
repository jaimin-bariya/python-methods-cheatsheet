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

## 📋 Dictionary Properties

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

### Example 2: Using `get` and `setdefault`
```python
d = {'a': 1}
print(d.get('b', 0))          # Output: 0 (default value)
d.setdefault('b', 2)          # Adds 'b': 2 if 'b' does not exist
print(d)                      # Output: {'a': 1, 'b': 2}
```

### Example 3: Iterating Over a Dictionary
```python
d = {'a': 1, 'b': 2}
for key, value in d.items():
    print(f"{key}: {value}")
# Output:
# a: 1
# b: 2
```

---

Continue exploring this repository for other data structures and their methods. 🚀
