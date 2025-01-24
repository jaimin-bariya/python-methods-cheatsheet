# Lists Methods and Properties Cheat Sheet

Python's **list** is an ordered, mutable sequence that is widely used for storing collections of items. Here are its most commonly used **methods** and **properties** along with examples to make them easy to understand.

---

## 🛠 List Methods

| **Method**         | **Description**                                    | **Example**                       |
|---------------------|----------------------------------------------------|-----------------------------------|
| `append(item)`      | Adds an item to the end of the list.               | `l.append(5)`                     |
| `extend(iterable)`  | Adds all elements of an iterable to the end.       | `l.extend([1, 2, 3])`             |
| `insert(index, item)`| Inserts an item at the specified index.            | `l.insert(1, "Hello")`            |
| `remove(item)`      | Removes the first occurrence of the specified item.| `l.remove(5)`                     |
| `pop(index=-1)`     | Removes and returns an item by index (default: last).| `l.pop()`                         |
| `clear()`           | Removes all items from the list.                  | `l.clear()`                       |
| `index(item)`       | Returns the index of the first occurrence of the item.| `l.index("Hello")`               |
| `count(item)`       | Returns the number of times an item appears in the list.| `l.count(5)`                   |
| `sort()`            | Sorts the list in ascending order (modifies in place).| `l.sort()`                       |
| `reverse()`         | Reverses the order of items in the list (in place).| `l.reverse()`                    |
| `copy()`            | Returns a shallow copy of the list.               | `copy_list = l.copy()`            |

---

## 📋 List Properties

| **Property**     | **Description**                   | **Example**             |
|-------------------|-----------------------------------|-------------------------|
| Mutable          | Lists can be modified after creation. | `l[0] = 10`            |
| Ordered          | Items in a list have a fixed order.   | `l = [1, 2, 3]`        |
| Allow Duplicates | Lists can contain duplicate values.   | `l = [1, 1, 2]`        |

---

## 💡 Examples

### Example 1: Using `append` and `extend`
```python
l = [1, 2, 3]
l.append(4)   # [1, 2, 3, 4]
l.extend([5, 6])  # [1, 2, 3, 4, 5, 6]
```

### Example 2: Using `sort` and `reverse`
```python
l = [3, 1, 4, 2]
l.sort()       # [1, 2, 3, 4]
l.reverse()    # [4, 3, 2, 1]
```

---

Continue exploring this repository for other data structures and their methods. 🚀
