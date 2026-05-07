# 📘 NumPy Day 1 — Introduction & Environment

---

## 📖 🔹 What is NumPy?

- 🧠 NumPy (Numerical Python) is a powerful Python library for numerical computing
- 📊 It helps you work with arrays (1D, 2D, 3D) efficiently
- ⚡ It performs fast mathematical operations on large datasets
- 🤖 It is widely used in Data Science, Machine Learning, and AI

---

## ❓ 🔹 Why NumPy?

- 🚀 Much faster than Python lists
- 🔢 Supports element-wise mathematical operations
- 📦 Handles large data efficiently
- 🤖 Essential for Machine Learning & Data Analysis
- 🧮 Built-in functions for complex calculations

---

## ⚠️ 🔹 Problem with Python List

```python
arr = [1, 2, 3]

print(arr * 5)
```

### ❌ Output:

```
[1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3]
```

- 😕 Instead of multiplying, it **repeats the list**
- ❌ Not suitable for mathematical operations

---

## ✅ 🔹 Solution with NumPy

```python
import numpy as np

arr = np.array([1, 2, 3])

print(arr * 5)
```

### ✅ Output:

```
[ 5 10 15]
```

- 🎯 Each element is multiplied individually
- ⚡ Fast and efficient

---

## ⚙️ 🔹 Installation & Import

### 📦 Install NumPy

```bash
pip install numpy
```

### 📥 Import NumPy

```python
import numpy as np
```

- 🔹 `np` is a standard short name (alias)

---

## 🧱 🔹 Syntax / Concept Section

- 🧩 `np.array()` → create a NumPy array
- 🔢 `arr * number` → element-wise multiplication
- ➕ `arr + number` → element-wise addition
- 📐 Supports multi-dimensional arrays

---

## 💻 🔹 Code Examples (Beginner Friendly)

---

### 📁 Example 1: Install & Import

```python
# Import NumPy library
import numpy as np

# Check version (optional)
print(np.__version__)
```

👉 🧠 Explanation:

- `import numpy as np` → loads NumPy
- `np.__version__` → shows installed version

---

### 📁 Example 2: Python List vs NumPy

```python
# Python list
arr = [1, 2, 3]

print(arr * 5)  # repeats list


# NumPy array
import numpy as np

arr_np = np.array([1, 2, 3])

print(arr_np * 5)  # multiplies elements
```

👉 🧠 Explanation:

- List → repeats values
- NumPy → multiplies each value individually

---

### 📁 Example 3: Array Creation

```python
import numpy as np

# 1D array
arr1 = np.array([1, 2, 3, 4, 5])
print(arr1)

# Check type
print(type(arr1))  # numpy.ndarray

# 2D array (matrix)
arr2 = np.array([
    [1, 2, 3],
    [4, 5, 6]
])
print(arr2)
```

👉 🧠 Explanation:

- `np.array()` creates array
- 1D = single row
- 2D = rows + columns (matrix)

---

### 📁 Example 4: Element-wise Operations

```python
import numpy as np

arr = np.array([1, 2, 3])

print(arr + 2)   # addition
print(arr * 3)   # multiplication
print(arr ** 2)  # square
```

👉 🧠 Explanation:

- NumPy automatically applies operation to **each element**
- No loop needed → faster code

---

### 📁 Example 5: List vs NumPy Operation

```python
# Python list
lst = [1, 2, 3]
lst_result = [x * 2 for x in lst]
print(lst_result)


# NumPy array
import numpy as np
arr = np.array([1, 2, 3])

print(arr * 2)
```

👉 🧠 Explanation:

- List → needs loop
- NumPy → direct operation

---

## 🌍 🔹 Real-Life Example

```python
import numpy as np

marks = np.array([50, 60, 70])

# Add bonus marks
updated_marks = marks + 5

print(updated_marks)
```

### ✅ Output:

```
[55 65 75]
```

👉 🧠 Explanation:

- Each student gets +5 marks
- NumPy applies it to all values automatically

---

## 🎯 🔹 Summary

- ✅ Learned what NumPy is
- ✅ Understood why NumPy is important
- ✅ Compared Python list vs NumPy array
- ✅ Learned how to create arrays
- ✅ Understood element-wise operations
- ✅ Practiced real-life example

---

# Author

**Engr. Md Monjur Bakth Mazumder**

🎓 Diploma in Computer Science and Technology — [Moulvibazar Polytechnic Institute](https://mpi.moulvibazar.gov.bd/)  
🎓 BSc in Computer Science & Engineering (CSE) (Ongoing) — [Sylhet International University](https://siu.edu.bd/)

📧 Email: monjurmbm404@gmail.com

### ⭐ If you find this helpful, don’t forget to **star** the repository!
