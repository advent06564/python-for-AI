# 📋 Syllabus — Module 1: Python Basics

**Week:** 1–2 | **Duration:** 1.5 weeks | **Phase:** 1 (Python Foundations)

---

## ⚡ **TL;DR**

Learn Python syntax, data types, loops, functions, and file I/O from scratch. No prior coding required. By the end, you'll write small utility scripts that work.

---

## 🎯 **Learning Objectives**

After this module, you will be able to:
- [ ] Declare variables and understand core data types (int, float, str, list, dict, tuple, set)
- [ ] Write conditional logic (if/elif/else) and loops (for, while)
- [ ] Define functions with parameters, arguments, and return values
- [ ] Work fluently with strings, lists, and dictionaries
- [ ] Import and use modules from Python's standard library

---

## 📚 **Topics Covered**

| Topic | Time | Subtopics |
|-------|------|-----------|
| **Variables & Types** | 2 hrs | int, float, str, bool, type conversion |
| **Operators** | 1 hr | arithmetic, comparison, logical, assignment |
| **Control Flow** | 2 hrs | if/elif/else, ternary operator |
| **Loops** | 2 hrs | for, while, break, continue, range() |
| **Functions** | 3 hrs | def, parameters, defaults, return, *args, **kwargs, scope |
| **Data Structures** | 3 hrs | lists, tuples, sets, dictionaries, indexing, slicing |
| **Strings** | 1.5 hrs | formatting, methods, f-strings |
| **File I/O** | 1.5 hrs | open(), read(), write(), context managers |
| **Error Handling** | 1 hr | try/except/finally, raising exceptions |
| **Modules** | 1 hr | import, os, math, random, json, datetime |

**Total:** ~17.5 hours (can be compressed to 10 hours if you already know some basics)

---

## 📖 **Free Resources**

### Primary

| Resource | Type | Time | URL |
|----------|------|------|-----|
| Official Python Tutorial (Chapters 3–10) | Docs | 4 hrs | https://docs.python.org/3/tutorial/ |
| Automate the Boring Stuff (Chapters 1–12) | Free Book | 6 hrs | https://automatetheboringstuff.com/ |
| freeCodeCamp Python (First 2 hrs) | YouTube | 2 hrs | https://youtu.be/rfscVS0vtbw |

### Supplementary

| Resource | Type | URL |
|----------|------|-----|
| W3Schools Python Interactive | Interactive | https://www.w3schools.com/python/ |
| Real Python Tutorials (beginner tag) | Articles | https://realpython.com/learning-paths/python-basics/ |
| Python Docs Quick Reference | Docs | https://docs.python.org/3/library/stdtypes.html |

---

## 💻 **Activities & Hands-On Practice**

### **Mini-Exercise 1: Hello, Variables** (30 min)
```python
# Declare variables of different types
name = "Alice"
age = 25
height = 5.8
is_student = True

# Print them
print(name, age, height, is_student)

# What's the type of each?
print(type(name))
```

**Your task:** Modify the code to print your own info.

---

### **Mini-Exercise 2: Conditionals** (30 min)
```python
# Check if age qualifies for voting
age = 18
if age >= 18:
    print("You can vote!")
else:
    print("You're too young.")
```

**Your task:** Add a new condition: if age < 13, print "You're a child."

---

### **Mini-Exercise 3: Loops** (45 min)
```python
# Print numbers 1 to 5
for i in range(1, 6):
    print(i)

# Count backwards
for i in range(10, 0, -1):
    print(i)

# While loop
count = 0
while count < 3:
    print(count)
    count += 1
```

**Your task:** Print the first 10 multiples of 3.

---

### **Mini-Exercise 4: Functions** (1 hr)
```python
# Define a simple function
def greet(name):
    return f"Hello, {name}!"

# Call it
print(greet("Alice"))

# Function with default arguments
def add(a, b=0):
    return a + b

print(add(5))      # Uses default b=0
print(add(5, 3))   # Overrides default
```

**Your task:** Write a function that takes two numbers and returns their product.

---

### **Mini-Exercise 5: Lists & Dictionaries** (1.5 hrs)
```python
# Lists
fruits = ["apple", "banana", "cherry"]
print(fruits[0])        # First element
print(len(fruits))      # Length
fruits.append("date")   # Add item
print(fruits)           # Print all

# Dictionaries
person = {
    "name": "Alice",
    "age": 25,
    "city": "NYC"
}
print(person["name"])   # Access by key
person["age"] = 26      # Update value
print(person)           # Print all
```

**Your task:** Create a dictionary with your favorite book, author, and year published.

---

### **Mini-Exercise 6: String Formatting** (30 min)
```python
# f-strings (modern, recommended)
name = "Bob"
age = 30
print(f"My name is {name} and I'm {age} years old.")

# .format() (older style)
print("My name is {} and I'm {} years old.".format(name, age))

# String methods
text = "hello world"
print(text.upper())           # HELLO WORLD
print(text.capitalize())      # Hello world
print("python".replace("p", "P"))  # Python
```

**Your task:** Use an f-string to print: "I am [age] years old and I live in [city]."

---

## 🛠️ **Projects (Build This Week)**

### **Project 1: CLI Calculator** (2–3 hours)
**Goal:** Build a command-line calculator that supports +, −, ×, ÷.

**Requirements:**
- Ask user for two numbers
- Ask user for operation (+, -, *, /)
- Perform calculation
- Print result
- Handle division by zero error

**Starter code:**
```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))
op = input("Enter operation (+, -, *, /): ")

# Your code here: perform calculation and print result
```

**Challenge:** Add a "history" feature that stores previous calculations.

---

### **Project 2: Word Counter** (2–3 hours)
**Goal:** Count word frequency in a text file.

**Requirements:**
- Create a text file (or download one)
- Read the file
- Count each word's frequency
- Print top 10 most common words

**Starter code:**
```python
filename = "sample.txt"
with open(filename, 'r') as file:
    text = file.read().lower()

# Your code here: count words
```

**Challenge:** Ignore common words (the, a, and, etc.) and print top 5.

---

### **Project 3: Password Generator** (1–2 hours)
**Goal:** Generate random secure passwords.

**Requirements:**
- Generate a password with uppercase, lowercase, digits
- Allow user to specify length
- Generate multiple passwords if requested

**Starter code:**
```python
import random
import string

length = int(input("Password length: "))
charset = string.ascii_letters + string.digits + string.punctuation

# Your code here: generate password
```

**Challenge:** Save generated passwords to a file.

---

## ✅ **Assessment / What to Submit**

By end of Week 2, submit:

1. **Completed Notebook** — `Week01.ipynb` with all exercises done
2. **Calculator Project** — Working code in `projects/calculator.py`
3. **Word Counter Project** — Code + sample output in `projects/word_counter/`
4. **Password Generator** — Code in `projects/password_generator.py`

**Submission format:**
- Commit to GitHub
- Include a README.md explaining how to run each project
- Add comments explaining your code

---

## 🎯 **Key Takeaways**

| Concept | What to Remember |
|---------|------------------|
| **Variables** | A named box that stores a value |
| **Data Types** | int, float, str, bool, list, dict, tuple, set |
| **Loops** | Repeat code: `for` (known iterations), `while` (until condition) |
| **Functions** | Reusable code blocks that take inputs and return outputs |
| **Lists** | Ordered, changeable, allow duplicates |
| **Dicts** | Key-value pairs, unordered (in older Python), changeable |
| **Error Handling** | `try/except` catches mistakes instead of crashing |

---

## 🚀 **Next Steps**

After completing this module:
1. Review your projects and clean up code
2. Add comments explaining what each section does
3. Move to **Module 2: Intermediate Python** (OOP, comprehensions, generators)

---

## 💡 **Common Mistakes to Avoid**

| Mistake | Why It's Wrong | Fix |
|---------|----------------|-----|
| `if x = 5:` | Single `=` is assignment, not comparison | Use `if x == 5:` |
| Forgetting `:` after if/for/while | Python syntax requires it | `if x > 0:` (note the colon) |
| Indentation errors | Python uses indentation to define blocks | Indent consistently (4 spaces) |
| `name[0]` on int | Can't index numbers | Convert to string first: `str(name)[0]` |
| Mutable default args | Defaults are set once, not per call | Avoid `def f(x=[]):` |

---

## 📞 **Getting Help**

- **Stuck?** → Check the official Python docs
- **Error message?** → Google it or check Stack Overflow
- **Concept unclear?** → Rewatch the YouTube video, try another source
- **Want to review?** → Look at the previous section's code

---

## 🎓 **Recommended Reading Order**

1. **Monday:** Variables, operators, types (2 hrs)
2. **Tuesday:** If/else, loops (2.5 hrs)
3. **Wednesday:** Functions (2 hrs)
4. **Thursday:** Lists & dictionaries (2 hrs)
5. **Friday:** Strings, file I/O, modules (2 hrs)
6. **Saturday–Sunday:** Build projects (6–8 hrs)

---

**Ready to start?** → [→ Open Week01.ipynb](../notebooks/Week01.ipynb)

---

*Module 1 Syllabus v1.0 | May 2026 | Python 3.11+*
