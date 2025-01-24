# Numbers Methods and Properties Cheat Sheet

Python's **numbers** include types like integers (`int`), floating-point numbers (`float`), and complex numbers (`complex`). These types have unique **methods** and **properties** that allow for powerful mathematical and computational operations.

---

## 🛠 Numbers Methods
Below are some common methods and functions used with numbers:

| **Function/Method**        | **Description**                                                                                 | **Example**                         |
|-----------------------------|-------------------------------------------------------------------------------------------------|-------------------------------------|
| `abs(x)`                   | Returns the absolute value of a number.                                                        | `abs(-5)` → `5`                    |
| `round(x, ndigits)`        | Rounds a number to a specified number of decimal places.                                       | `round(3.14159, 2)` → `3.14`       |
| `pow(x, y)`                | Returns `x` raised to the power of `y`.                                                        | `pow(2, 3)` → `8`                  |
| `divmod(a, b)`             | Returns a tuple `(quotient, remainder)` from dividing `a` by `b`.                              | `divmod(10, 3)` → `(3, 1)`         |
| `int(x)`                   | Converts a number or string to an integer.                                                     | `int(3.9)` → `3`                   |
| `float(x)`                 | Converts a number or string to a floating-point number.                                        | `float(5)` → `5.0`                 |
| `complex(re, im)`          | Creates a complex number with real and imaginary parts.                                        | `complex(2, 3)` → `(2+3j)`         |

---

## 🔢 Number Properties

| **Type**       | **Description**                                                               | **Example**                 |
|-----------------|-------------------------------------------------------------------------------|-----------------------------|
| Integer (`int`) | Whole numbers, positive or negative, with no decimal point.                  | `x = 10`                   |
| Float (`float`) | Numbers with a decimal point or in scientific notation.                      | `x = 3.14`                 |
| Complex (`complex`) | Numbers with a real part and an imaginary part.                             | `x = 1 + 2j`               |

---

## 📋 Number Operations and Usage

| **Operation**       | **Symbol/Function**       | **Example**                         |
|----------------------|---------------------------|-------------------------------------|
| Addition            | `+`                       | `5 + 3` → `8`                      |
| Subtraction         | `-`                       | `10 - 4` → `6`                     |
| Multiplication      | `*`                       | `2 * 3` → `6`                      |
| Division            | `/`                       | `7 / 2` → `3.5`                    |
| Floor Division      | `//`                      | `7 // 2` → `3`                     |
| Modulus             | `%`                       | `7 % 2` → `1`                      |
| Exponentiation      | `**`                      | `2 ** 3` → `8`                     |

---

## 💡 Examples

### Example 1: Basic Arithmetic
```python
x = 10
y = 3
print(x + y)         # Output: 13
print(x ** y)        # Output: 1000
```

### Example 2: Working with Floats
```python
pi = 3.14159
print(round(pi, 2))  # Output: 3.14
```

### Example 3: Using Complex Numbers
```python
z = complex(2, 3)
print(z.real)        # Output: 2.0
print(z.imag)        # Output: 3.0
```

---

Numbers in Python are powerful and versatile. With these methods and properties, you can perform everything from basic arithmetic to complex mathematical operations. 🚀
