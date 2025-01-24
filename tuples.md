# Tuples Methods and Properties Cheat Sheet

Python's **tuple** is an ordered, immutable sequence that is commonly used for fixed collections of items. While tuples are less flexible than lists, they have their own advantages, like being hashable and lightweight. Here are the **methods** and **properties** of tuples, along with examples.

---

## 🛠 Tuple Methods

| **Method**         | **Description**                                    | **Example**                       |
|---------------------|----------------------------------------------------|-----------------------------------|
| `count(item)`       | Returns the number of times an item appears in the tuple. | `t.count(5)`                     |
| `index(item)`       | Returns the index of the first occurrence of the item.     | `t.index("Hello")`              |

> Note: Tuples have limited methods since they are immutable.

---

## 📋 Tuple Properties

| **Property**     | **Description**                   | **Example**             |
|-------------------|-----------------------------------|-------------------------|
| Immutable         | Tuples cannot be modified after creation. | `t[0] = 10  # Error`   |
| Ordered           | Items in a tuple have a fixed order.       | `t = (1, 2, 3)`        |
| Allow Duplicates  | Tuples can contain duplicate values.       | `t = (1, 1, 2)`        |
| Hashable          | Tuples can be used as keys in dictionaries (if they only contain hashable items). | `d = {(1, 2): "value"}` |

---

## 💡 Examples

### Example 1: Basic Tuple Operations
```python
t = (1, 2, 3, 2)
print(t.count(2))    # 2
print(t.index(3))    # 2
```

### Example 2: Immutability of Tuples
```python
t = (1, 2, 3)
t[0] = 5   # This will raise a TypeError because tuples are immutable.
```

### Example 3: Using Tuples as Dictionary Keys
```python
coords = {(0, 0): "Origin", (1, 2): "Point A"}
print(coords[(1, 2)])   # "Point A"
```

---

Continue exploring this repository for other data structures and their methods. 🚀
