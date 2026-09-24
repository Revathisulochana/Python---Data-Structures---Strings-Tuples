# Python Assignment 1 – Data Structures: Strings & Tuples

This assignment covers basic string operations (concatenation, slicing, methods) and tuple operations (creation, modification, access) in Python.

---

## Table of Contents

1. [Strings](#strings)
   - [1. String Concatenation](#1-string-concatenation)
   - [2. String Slicing and Indexing](#2-string-slicing-and-indexing)
   - [3. String Methods](#3-string-methods)
2. [Tuples](#tuples)

---

## Strings

### 1. String Concatenation

Join a greeting, a user-entered name and a welcome message into one sentence.

```python
# 1. String Concatenation:

Text = "Hello "
name = input("Enter your name:")
Welcome = ("Welcome to Python programming")

print(Text + name + "," + Welcome)
```

**Output**

```
Enter your name:Revathi
Hello Revathi,Welcome to Python programming
```

---

### 2. String Slicing and Indexing

```python
# 2. String Slicing and Indexing:

text = "Hello Revathi,Welcome to Python programming"

# a. Print the first character of the string.
print(text[0])

# b. Print the last character of the string.
print(text[42])
print(text[-1])

# c. Print the first 5 characters of the string.
print(text[0:5])

# d. Print the last 11 characters of the string.
print(text[-11:])

# e. Print the string in reverse.
print(text[::-1])

# f. Use slicing and print the word "Python" from the existing string.
print(text[-18:-12])
print(text[25:31])
```

**Output**

```
H
g
g
Hello
programming
gnimmargorp nohtyP ot emocleW,ihtaveR olleH
Python
Python
```

**Notes**

| Expression | Meaning |
|------------|---------|
| `text[0]` | First character (index starts at 0) |
| `text[-1]` | Last character (negative index counts from the end) |
| `text[0:5]` | Characters from index 0 up to (not including) 5 |
| `text[-11:]` | Last 11 characters |
| `text[::-1]` | Whole string reversed (step of -1) |

---

### 3. String Methods

```python
# 3. String Methods:

strM = "Python beginner tutorial"

# a. Convert the sentence to uppercase.
print(strM.upper())

# b. Convert the sentence to lowercase.
print(strM.lower())

# c. Use capitalize and return the sentence to the original input form.
str = "PYTHON BEGINNER TUTORIAL"
print(str.capitalize())

# d. Count the total number of occurrences of character 't' in the string.
print(strM.count("t"))

# e. Replace all occurrences of "Python" with "Data Analytics"
strM = "Python beginner tutorial"
print(strM.replace("Python", "Data Analytics"))
```

**Output**

```
PYTHON BEGINNER TUTORIAL
python beginner tutorial
Python beginner tutorial
3
Data Analytics beginner tutorial
```

---

## Tuples

Creation, modification (by building new tuples) and access.

```python
# Tuples (Creation, Modification and Access):

tuple1 = 10, 20, 30
tuple2 = 40, 50, 60

# a. Concatenate the two tuples and store it in "t_combine"
t_combine = tuple1 + tuple2
print(t_combine)

# b. Repeat the elements of "t_combine" 3 times
print(t_combine * 3)

# c. Access the 3rd element from "t_combine"
print(t_combine[2])

# d. Access the first three elements from "t_combine"
print(t_combine[0:3])

# e. Access the last three elements from "t_combine"
print(t_combine[-3:])
```

**Output**

```
(10, 20, 30, 40, 50, 60)
(10, 20, 30, 40, 50, 60, 10, 20, 30, 40, 50, 60, 10, 20, 30, 40, 50, 60)
30
(10, 20, 30)
(40, 50, 60)
```

---

## Concepts Covered

- String concatenation with `+`
- Indexing (positive and negative) and slicing `[start:stop:step]`
- String methods: `upper()`, `lower()`, `capitalize()`, `count()`, `replace()`
- Tuple concatenation (`+`), repetition (`*`), indexing and slicing
- Tuples are immutable, so "modifying" one means creating a new tuple



Requires Python 3.x. No external libraries needed.
