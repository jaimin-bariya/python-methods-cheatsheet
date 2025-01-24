# Sets Methods and Properties Cheat Sheet

Python's **set** is a mutable, unordered collection of unique elements. Sets are optimized for membership checks and mathematical set operations. Here's a comprehensive list of **methods** and **properties** for sets, along with examples.

---

## 🛠 Set Methods

| **Method**                   | **Description**                                                                 | **Example**                           |
|-------------------------------|---------------------------------------------------------------------------------|---------------------------------------|
| `add(item)`                  | Adds an element to the set.                                                    | `s.add(10)`                           |
| `clear()`                    | Removes all elements from the set.                                             | `s.clear()`                           |
| `copy()`                     | Returns a shallow copy of the set.                                             | `new_set = s.copy()`                  |
| `difference(other_set)`      | Returns a set containing elements in the set but not in the other set.         | `s1.difference(s2)`                   |
| `difference_update(other_set)` | Removes elements found in another set from the original set.                   | `s1.difference_update(s2)`            |
| `discard(item)`              | Removes the specified element without raising an error if it doesn't exist.    | `s.discard(10)`                       |
| `intersection(other_set)`    | Returns a set containing elements common to both sets.                         | `s1.intersection(s2)`                 |
| `intersection_update(other_set)` | Updates the set with elements common to both sets.                            | `s1.intersection_update(s2)`          |
| `isdisjoint(other_set)`      | Returns `True` if the sets have no elements in common.                         | `s1.isdisjoint(s2)`                   |
| `issubset(other_set)`        | Returns `True` if the set is a subset of another set.                          | `s1.issubset(s2)`                     |
| `issuperset(other_set)`      | Returns `True` if the set is a superset of another set.                        | `s1.issuperset(s2)`                   |
| `pop()`                      | Removes and returns a random element from the set.                             | `s.pop()`                             |
| `remove(item)`               | Removes the specified element, raises an error if it doesn't exist.            | `s.remove(10)`                        |
| `symmetric_difference(other_set)` | Returns a set with elements in either set but not both.                      | `s1.symmetric_difference(s2)`         |
| `symmetric_difference_update(other_set)` | Updates the set to include elements in either set but not both.           | `s1.symmetric_difference_update(s2)`  |
| `union(other_set)`           | Returns a set containing all elements from both sets.                          | `s1.union(s2)`                        |
| `update(other_set)`          | Adds elements from another set to the original set.                            | `s1.update(s2)`                       |

---

## 📋 Set Properties

| **Property**       | **Description**                                           | **Example**                 |
|---------------------|-----------------------------------------------------------|-----------------------------|
| Mutable            | Sets can be modified after creation.                      | `s.add(10)`                 |
| Unordered          | Items are not stored in a specific order.                  | `s = {1, 2, 3}`             |
| Unique Items Only  | Sets automatically discard duplicate values.               | `s = {1, 1, 2}` (Keeps one) |
| Hashable Elements  | Set elements must be immutable (e.g., strings, numbers, tuples). | `s = {(1, 2), 3}`          |

---

## 💡 Examples

### Example 1: Basic Set Operations
```python
s = {1, 2, 3}
s.add(4)             # Adds 4 to the set
print(s)             # Output: {1, 2, 3, 4}
s.remove(2)          # Removes 2 from the set
print(s)             # Output: {1, 3, 4}
```

### Example 2: Mathematical Set Operations
```python
s1 = {1, 2, 3}
s2 = {3, 4, 5}
print(s1.union(s2))                # Output: {1, 2, 3, 4, 5}
print(s1.intersection(s2))         # Output: {3}
print(s1.difference(s2))           # Output: {1, 2}
print(s1.symmetric_difference(s2)) # Output: {1, 2, 4, 5}
```

### Example 3: Checking Subset and Superset
```python
s1 = {1, 2}
s2 = {1, 2, 3}
print(s1.issubset(s2))   # Output: True
print(s2.issuperset(s1)) # Output: True
```

---

Continue exploring this repository for other data structures and their methods. 🚀
