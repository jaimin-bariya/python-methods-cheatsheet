# 📜 Python Special (Dunder) Methods Cheat Sheet

Python's **special methods** (also called "dunder methods" because they are surrounded by double underscores) give classes built-in behavior when they interact with Python’s syntax or standard functions. These methods allow you to define how your objects respond to specific operations, such as addition, string representation, or comparison.

---

## 🛠 Magic Methods Categories

### 1. **Initialization and Representation**
| **Method**        | **Purpose**                       | **Example**               |
|--------------------|-----------------------------------|---------------------------|
| `__init__`         | Object initialization            | `def __init__(self, ...)` |
| `__repr__`         | Official string representation   | `repr(obj)`              |
| `__str__`          | Informal string representation   | `str(obj)`               |
| `__del__`          | Cleanup when object is deleted   | `del obj`                |

### 2. **Arithmetic Operators**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__add__`          | Define addition (`+`)            | `obj1 + obj2`           |
| `__sub__`          | Define subtraction (`-`)         | `obj1 - obj2`           |
| `__mul__`          | Define multiplication (`*`)      | `obj1 * obj2`           |
| `__truediv__`      | Define true division (`/`)        | `obj1 / obj2`           |
| `__floordiv__`     | Define floor division (`//`)     | `obj1 // obj2`          |
| `__mod__`          | Define modulus (`%`)             | `obj1 % obj2`           |
| `__pow__`          | Define power (`**`)              | `obj1 ** obj2`          |

### 3. **Comparison Operators**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__eq__`           | Equal to (`==`)                  | `obj1 == obj2`          |
| `__ne__`           | Not equal to (`!=`)              | `obj1 != obj2`          |
| `__lt__`           | Less than (`<`)                  | `obj1 < obj2`           |
| `__le__`           | Less than or equal to (`<=`)     | `obj1 <= obj2`          |
| `__gt__`           | Greater than (`>`)               | `obj1 > obj2`           |
| `__ge__`           | Greater than or equal to (`>=`)  | `obj1 >= obj2`          |

### 4. **Container-Like Behavior**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__getitem__`      | Retrieve item by key/index       | `obj[key]`              |
| `__setitem__`      | Set item by key/index            | `obj[key] = value`      |
| `__delitem__`      | Delete item by key/index         | `del obj[key]`          |
| `__len__`          | Return length of container       | `len(obj)`              |
| `__contains__`     | Check membership (`in`)          | `item in obj`           |
| `__iter__`         | Define iteration behavior        | `for x in obj:`         |

### 5. **Attribute Access**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__getattr__`      | Access attribute dynamically     | `obj.attr`              |
| `__setattr__`      | Set attribute dynamically        | `obj.attr = value`      |
| `__delattr__`      | Delete attribute dynamically     | `del obj.attr`          |
| `__dir__`          | Customize `dir()` result         | `dir(obj)`              |

### 6. **Call Behavior**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__call__`         | Make object callable             | `obj()`                 |

### 7. **Context Manager Support**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__enter__`        | Define enter behavior            | `with obj:`             |
| `__exit__`         | Define exit behavior             | `with obj:`             |

### 8. **Other Useful Methods**
| **Method**        | **Purpose**                       | **Example**             |
|--------------------|-----------------------------------|-------------------------|
| `__hash__`         | Compute object’s hash            | `hash(obj)`             |
| `__bool__`         | Define truth value of object     | `bool(obj)`             |
| `__format__`       | Customize string formatting      | `format(obj, spec)`     |
| `__sizeof__`       | Return memory size of object     | `sys.getsizeof(obj)`    |

---

## 🎯 How to Use Special Methods

Here’s an example of customizing a class with special methods:

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __add__(self, other):
        return Vector(self.x + other.x, self.y + other.y)

    def __repr__(self):
        return f"Vector({self.x}, {self.y})"

v1 = Vector(1, 2)
v2 = Vector(3, 4)
print(v1 + v2)  # Output: Vector(4, 6)
```

---

### 🌟 Contribute
If you find this cheat sheet helpful or have suggestions, feel free to contribute or raise issues in the repository!

Happy Coding! 😄
