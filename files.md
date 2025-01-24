# Files Methods and Properties Cheat Sheet

Python provides extensive support for file handling, enabling efficient interaction with files for reading, writing, and manipulation. Below is a cheat sheet summarizing commonly used **file methods** and properties.

---

## 🛠 File Methods

| **Method**             | **Description**                                                                                      | **Example**                                  |
|------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------|
| `open(filename, mode)` | Opens a file in the specified mode (`r`, `w`, `a`, `b`, etc.) and returns a file object.             | `file = open("data.txt", "r")`             |
| `read(size)`           | Reads the file content up to the specified size (or all if size is omitted).                        | `data = file.read()`                         |
| `readline()`           | Reads a single line from the file.                                                                  | `line = file.readline()`                     |
| `readlines()`          | Reads all lines from the file as a list.                                                            | `lines = file.readlines()`                   |
| `write(content)`       | Writes the specified string to the file.                                                           | `file.write("Hello, World!\n")`            |
| `writelines(lines)`    | Writes a list of strings to the file.                                                               | `file.writelines(["Line 1\n", "Line 2\n"])` |
| `close()`              | Closes the file and releases resources.                                                            | `file.close()`                               |
| `seek(offset)`         | Moves the file pointer to the specified offset.                                                     | `file.seek(0)`                               |
| `tell()`               | Returns the current position of the file pointer.                                                   | `position = file.tell()`                     |
| `flush()`              | Flushes the file’s write buffer, forcing the write to disk.                                         | `file.flush()`                               |

---

## 📂 File Modes

| **Mode**  | **Description**                                                                 |
|-----------|---------------------------------------------------------------------------------|
| `r`       | Read mode (default). Opens the file for reading; raises error if the file doesn’t exist. |
| `w`       | Write mode. Opens the file for writing, truncating its contents if it exists.           |
| `a`       | Append mode. Opens the file for writing, appending new content to the end.             |
| `x`       | Exclusive creation mode. Creates a file; raises error if the file already exists.      |
| `b`       | Binary mode. Used with other modes to handle binary files.                            |
| `t`       | Text mode (default). Used with other modes to handle text files.                     |

---

## 📋 File Properties

| **Property**           | **Description**                                                                                      | **Example**                          |
|------------------------|------------------------------------------------------------------------------------------------------|--------------------------------------|
| `file.closed`          | Returns `True` if the file is closed, otherwise `False`.                                             | `print(file.closed)`                 |
| `file.mode`            | Returns the mode in which the file was opened (`r`, `w`, etc.).                                      | `print(file.mode)`                   |
| `file.name`            | Returns the name of the file.                                                                        | `print(file.name)`                   |
| `file.encoding`        | Returns the file’s encoding (for text files).                                                        | `print(file.encoding)`               |

---

## 💡 Examples

### Example 1: Reading a File
```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)  # Prints the entire content of the file
```

### Example 2: Writing to a File
```python
with open("output.txt", "w") as file:
    file.write("This is a test file.\n")
    file.write("Python file handling is simple.")
```

### Example 3: Appending to a File
```python
with open("output.txt", "a") as file:
    file.write("\nAppending new content.")
```

### Example 4: Iterating Through Lines
```python
with open("example.txt", "r") as file:
    for line in file:
        print(line.strip())
```

---

File handling in Python is simple yet powerful, with robust methods and properties to perform various operations. Make sure to close files or use the `with` statement for better resource management. 🚀
