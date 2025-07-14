# 🐍 Python Sets – Complete Guide

## 📘 Introduction

> *A `set` in Python is an **unordered**, **unindexed**, and **mutable** collection that stores **unique** items. Sets are useful for eliminating duplicates and performing mathematical set operations.*

---

## 🔧 Set Creation

### 📌 **Definition**

> *You can create a set using curly braces `{}` or the built-in `set()` function.*

### 💻 **Example Code:**

```python
# Creating a set
numbers = set([1, 2, 2, 3])
print(numbers)
```

### 🟩 **Output:**

```
{1, 2, 3}
```

---

## ➕ Adding Elements

### 📌 **Definition**

> *Use `add()` to insert a single element. Use `update()` to insert multiple elements.*

### 💻 **Example Code (`add`)**

```python
s = {1, 2}
s.add(3)
print(s)
```

### 🟩 **Output:**

```
{1, 2, 3}
```

### 💻 **Example Code (`update`)**

```python
s = {1, 2}
s.update([3, 4, 5])
print(s)
```

### 🟩 **Output:**

```
{1, 2, 3, 4, 5}
```

---

## ➖ Removing Elements

### 📌 **Definition**

> *Use `remove()` to delete a specific element (error if not found). Use `discard()` to delete safely (no error if not found).*

### 💻 **Example Code (`remove`)**

```python
my_set = {1, 2, 3}
my_set.remove(2)
print(my_set)
```

### 🟩 **Output:**

```
{1, 3}
```

### 💻 **Example Code (`discard`)**

```python
my_set = {1, 2, 3}
my_set.discard(4)
print(my_set)
```

### 🟩 **Output:**

```
{1, 2, 3}
```

---

## 🔁 Set Operations

### 📌 **Definition**

> *Set operations are used to perform mathematical operations between sets such as union, intersection, difference, and symmetric difference.*

```python
a = {1, 2, 3}
b = {3, 4, 5}
```

### 🟢 **Union**

> *Returns a new set with all elements from both sets, removing duplicates. You can use `union()` or the `|` operator.*

```python
print(a.union(b))       # or a | b
```

```
{1, 2, 3, 4, 5}
```

### 🟢 **Intersection**

> *Returns a set of elements that are common to both sets. You can use `intersection()` or the `&` operator.*

```python
print(a.intersection(b))  # or a & b
```

```
{3}
```

### 🟢 **Difference**

> *Returns a set with elements that are in the first set but not in the second. Use `difference()` or the `-` operator.*

```python
print(a.difference(b))    # or a - b
```

```
{1, 2}
```

### 🟢 **Symmetric Difference**

> *Returns a set with elements in either of the sets, but not in both. Use `symmetric_difference()` or the `^` operator.*

```python
print(a.symmetric_difference(b))  # or a ^ b
```

```
{1, 2, 4, 5}
```

---

## 📊 Set Comparison Methods

> Below are commonly used set comparison methods in Python. Each method checks the relationship between two sets and returns a boolean value.

---

<div style="border: 2px solid #4CAF50; padding: 16px; border-radius: 10px; background-color: #f0fff4;">

### 🧩 `issubset()` - Subset Checker 🧩

#### 📌 Definition

> *Checks if all elements of the calling set are present in another set.*

#### 💻 Example Code

```python
a = {1, 2}
b = {1, 2, 3}
print(a.issubset(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

🎯 *Since all elements of `a` (1 and 2) are in `b`, `issubset()` returns `True`.*

</div>

---

<div style="border: 2px solid #2196F3; padding: 16px; border-radius: 10px; background-color: #f0f8ff;">

### 🛡️ `issuperset()` - Superset Defender 🛡️

#### 📌 Definition

> *Checks if the calling set contains all elements of another set.*

#### 💻 Example Code

```python
a = {1, 2, 3}
b = {1, 2}
print(a.issuperset(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

🛡️ *Since `a` has all elements of `b`, `issuperset()` returns `True`.*

</div>

---

<div style="border: 2px solid #FF5722; padding: 16px; border-radius: 10px; background-color: #fff3e0;">

### 🚫 `isdisjoint()` - No Common Ground 🚫

#### 📌 Definition

> *Checks if two sets have **no elements in common**.*

#### 💻 Example Code

```python
a = {1, 2}
b = {3, 4}
print(a.isdisjoint(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

🧯 *Since `a` and `b` share no common elements, `isdisjoint()` returns `True`.*

</div>

---

### 🛡️ `issuperset()` - Superset Defender 🛡️

#### 📌 Definition

> *Checks if the calling set contains all elements of another set.*

#### 💻 Example Code

```python
a = {1, 2, 3}
b = {1, 2}
print(a.issuperset(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

🛡️ *Since `a` has all elements of `b`, `issuperset()` returns `True`.*

---

### 🚫 `isdisjoint()` - No Common Ground 🚫

#### 📌 Definition

> *Checks if two sets have **no elements in common**.*

#### 💻 Example Code

```python
a = {1, 2}
b = {3, 4}
print(a.isdisjoint(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

🧯 *Since `a` and `b` share no common elements, `isdisjoint()` returns `True`.*

---

### 🔸 `issubset()`

#### 📌 Definition

> *Checks if all elements of the calling set are present in another set.*

#### 💻 Example Code

```python
a = {1, 2}
b = {1, 2, 3}
print(a.issubset(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

> *Since all elements of `a` (1 and 2) are in `b`, `issubset()` returns `True`.*

---

### 🔸 `issuperset()`

#### 📌 Definition

> *Checks if the calling set contains all elements of another set.*

#### 💻 Example Code

```python
a = {1, 2, 3}
b = {1, 2}
print(a.issuperset(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

> *Since `a` has all elements of `b`, `issuperset()` returns `True`.*

---

### 🔸 `isdisjoint()`

#### 📌 Definition

> *Checks if two sets have **no elements in common**.*

#### 💻 Example Code

```python
a = {1, 2}
b = {3, 4}
print(a.isdisjoint(b))
```

#### 🟩 Output

```
True
```

#### 🧠 Explanation

> *Since `a` and `b` share no common elements, the result is `True`.*

---

## 🔄 Set Comprehension

### 📌 **Definition**

> *Set comprehension is used to create a set using an expression inside curly braces `{}`.*

### 💻 **Example Code:**

```python
squares = {x**2 for x in range(5)}
print(squares)
```

### 🟩 **Output:**

```
{0, 1, 4, 9, 16}
```

---

## 🫒 Frozen Sets

### 📌 **Definition**

> *A `frozenset` is an **immutable** version of a set. You cannot modify it after creation.*

### 💻 **Example Code:**

```python
fs = frozenset([1, 2, 3])
print(fs)
```

### 🟩 **Output:**

```
frozenset({1, 2, 3})
```

---

## 📚 Set Method Summary

| **Method**                     | **Description**                                       |                    |
| ------------------------------ | ----------------------------------------------------- | ------------------ |
| `add(x)`                       | Adds `x` to the set                                   |                    |
| `update(iterable)`             | Adds multiple elements                                |                    |
| `remove(x)`                    | Removes `x`; error if not found                       |                    |
| `discard(x)`                   | Removes `x`; no error if not found                    |                    |
| `pop()`                        | Removes and returns a random element                  |                    |
| `clear()`                      | Removes all elements                                  |                    |
| `union(other)` / \`            | \`                                                    | Combines both sets |
| `intersection(other)` / `&`    | Common elements                                       |                    |
| `difference(other)` / `-`      | Elements only in the first set                        |                    |
| `symmetric_difference()` / `^` | Elements not common to both sets                      |                    |
| `issubset(other)`              | True if all elements are in the other set             |                    |
| `issuperset(other)`            | True if all elements of the other set are in this set |                    |
| `isdisjoint(other)`            | True if no elements are common                        |                    |

---

## ✅ Conclusion

> *Python sets are powerful for ensuring uniqueness, performing fast membership tests, and doing mathematical operations. Use sets when you need **speed**, **uniqueness**, or **set algebra**.*
