📘 Python 30-Day Syllabus

🎬 **DAY 06 – PYTHON OPERATORS (Full Script)**

---

🎯 **HOOK (First 5 seconds)**

“Do you think Python is just for printing Hello World? 😄
What if I show you… Python can work like a powerful calculator and decision maker? 🔥”

---

👋 **INTRO**

Hello friends… welcome back to Day 06 🚀

In today’s session, we are going to learn:

👉 Python Operators

Operators are very very important…
Without operators, we cannot perform any operations in programming.

---

# 🧠 **PART 1: What is an Operator?**

👉 Simple definition:

“Operator is a symbol which performs an operation on values”

Example:

👉 10 + 20

Here:

* 10, 20 → operands
* * → operator

---

# ➕ **PART 2: Arithmetic Operators**

Let’s start with basic operators:

```python
a = 10
b = 3

print(a + b)   # Addition
print(a - b)   # Subtraction
print(a * b)   # Multiplication
print(a / b)   # Division
print(a % b)   # Modulus
print(a // b)  # Floor Division
print(a ** b)  # Power
```

---

💡 **Explain Like This:**

👉 `/` gives decimal
👉 `//` removes decimal

Example:
👉 10 / 3 = 3.33
👉 10 // 3 = 3

---

😂 **Fun Line**

“Normal division is like real life…
Floor division is like strict teacher… no decimals allowed 😄”

---

# 🔍 **PART 3: Comparison Operators**

Used to compare values:

```python
a = 10
b = 20

print(a > b)
print(a < b)
print(a == b)
print(a != b)
```

---

👉 Output is always:

✔ True or False (Boolean)

---

💡 **Real-Life Example**

“Checking marks…
Is marks > 50? → pass or fail”

---

# 🔗 **PART 4: Logical Operators**

```python
age = 20
has_id = True

print(age >= 18 and has_id)
```

---

👉 Explain:

* `and` → both must be true
* `or` → at least one true
* `not` → reverse

---

😂 **Fun Line**

“and condition is like strict parents… both conditions must be satisfied 😄”

---

# 🆔 **PART 5: Identity Operators**

```python
a = 10
b = 10

print(a is b)
print(a is not b)
```

👉 Checks memory (same object or not)

---

# 📦 **PART 6: Membership Operators**

```python
name = "python"

print("p" in name)
print("z" not in name)
```

👉 Used in strings, lists

---

# 🚀 🎯 **MINI PROJECT: SIMPLE CALCULATOR**

Now let’s build something practical.

```python
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
```

---

👉 Say:

“This is how calculator apps start… simple logic, but powerful idea 🔥”

---

# 🚀 🎯 **PROJECT 2: EVEN OR ODD CHECKER**

```python
num = int(input("Enter a number: "))

if num % 2 == 0:
    print("Even Number ✅")
else:
    print("Odd Number ❌")
```

---

💡 Explain:

“% gives remainder…
If remainder = 0 → even number”

---

# 🚀 🎯 **PROJECT 3: LOGIN CHECK (REAL-WORLD)**

```python
username = input("Enter username: ")
password = input("Enter password: ")

if username == "admin" and password == "1234":
    print("Login Success 🔥")
else:
    print("Invalid Credentials ❌")
```

---

👉 Say:

“This is exactly how apps validate login internally”

---

# 🎯 **ENDING**

Today we learned:

✔ Arithmetic Operators
✔ Comparison Operators
✔ Logical Operators
✔ Real-world projects

---

👉 Practice is very important

“Watching coding is like watching gym videos…
You won’t get results unless you practice 😄”

---

💬 Comment “DAY06” if you completed 💪🔥

See you in Day 07 🚀
