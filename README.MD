📘 Python 30-Day Syllabus

🎬 **DAY 07 – LISTS (Advanced Data Structures – Part 1)**

---

🎯 **HOOK (First 5–7 sec)**

“Till now we stored only one value in one variable…
But what if I want to store 100 values? 😳

That’s where Lists come into picture 🔥”

---

👋 **INTRO**

Hello friends, welcome back to Day 07 🚀

Today we are starting:

👉 Advanced Data Structures

And in today’s session, we will focus on:

👉 **Lists in Python**

---

# 🧠 **PART 1: What is a List?**

👉 Definition:

“A list is a collection of multiple values stored in a single variable”

---

### 💻 Example:

```python
numbers = [10, 20, 30, 40]
```

---

💡 Say:

“Instead of creating 4 variables… we can store everything in one list”

---

# 🧠 **PART 2: List with Different Data Types**

```python
data = [10, 3.5, "Python", True]
```

👉 Explain:

“List can store multiple data types at the same time”

---

# 🧠 **PART 3: Accessing Elements (Indexing)**

```python
names = ["Rahul", "Ravi", "Priya"]

print(names[0])
print(names[-1])
```

---

💡 Explain:

0 → first
-1 → last

---

😂 Fun Line:

“Negative indexing is like going from backside 😄”

---

# 🧠 **PART 4: Slicing Lists**

```python
nums = [10, 20, 30, 40, 50]

print(nums[1:4])
```

---

👉 Explain:

“Slicing means taking a portion of list”

---

# 🧠 **PART 5: Modify List**

```python
nums = [10, 20, 30]

nums[1] = 99
print(nums)
```

👉 Lists are **mutable** (can change)

---

# 🧠 **PART 6: Adding Elements**

```python
nums = [10, 20]

nums.append(30)
nums.insert(1, 15)

print(nums)
```

---

# 🧠 **PART 7: Removing Elements**

```python
nums = [10, 20, 30]

nums.remove(20)
nums.pop()

print(nums)
```

---

# 🧠 **PART 8: Loop Through List**

```python
nums = [10, 20, 30]

for i in nums:
    print(i)
```

---

💡 Say:

“This is how real applications process data”

---

# 🚀 🎯 **MINI PROJECT: STUDENT MARKS SYSTEM**

👉 Very powerful example

```python
marks = []

n = int(input("Enter number of students: "))

for i in range(n):
    m = int(input("Enter marks: "))
    marks.append(m)

print("All Marks:", marks)

print("Maximum Marks:", max(marks))
print("Minimum Marks:", min(marks))
print("Total Marks:", sum(marks))
print("Average:", sum(marks)/len(marks))
```

---

# 🎯 🗣️ **Explain Like This**

👉 Say:

“This is exactly how systems store and process student data…
We are doing same thing using lists 🔥”

---

# 😂 FUN LINE

“List is like your friend group…
You can add, remove, and manage easily 😄”

---

# 🎯 **ENDING**

Today we learned:

✔ What is List
✔ Indexing & Slicing
✔ Add & Remove
✔ Looping
✔ Real-world mini project

---

👉 Practice is very important

💬 Comment “DAY07” if completed 💪🔥

See you in next session 🚀
