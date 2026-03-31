📘 Python 30-Day Syllabus
Day09

🧠 ✅ What is Set?

👉 If we want to represent a group of unique values as a single entity, then we use Set

⚡ Key Properties of Set

✔ Duplicates are NOT allowed
✔ Insertion order is NOT preserved
✔ Indexing & slicing are NOT allowed
✔ Set is mutable (can modify)

💻 ✅ How to Create Set
s = {10, 20, 30, 40}
print(s)
print(type(s))
❗ Duplicate Example
s = {10, 20, 20, 30}
print(s)

👉 Output:

{10, 20, 30}

👉 💡 Duplicate automatically removed 🔥

🛠️ ✅ Important Functions of Set
🔹 1. add()

👉 Adds single element

s = {10, 20, 30}
s.add(50)
print(s)
🔹 2. update()

👉 Adds multiple elements

s = {10, 20}
l = [30, 40, 50]

s.update(l, range(2))
print(s)
🔹 3. copy()

👉 Creates duplicate set

s = {10, 20, 30}
s1 = s.copy()

print(s1)
🔹 4. pop()

👉 Removes random element

s = {10, 20, 30}
print(s.pop())
print(s)

👉 💡 Random element removed 😳

🔹 5. remove()

👉 Removes specific element

s = {10, 20, 30}
s.remove(20)
print(s)
🔢 ✅ Mathematical Operations
🔹 1. union()

👉 Combine two sets

s = {10, 20, 30}
s1 = {30, 40, 50}

print(s.union(s1))
🔹 2. intersection()

👉 Common elements

s = {10, 20, 30}
s1 = {20, 30, 40}

print(s.intersection(s1))
🔹 3. difference()

👉 Unique elements

s = {10, 20, 30}
s1 = {20, 30, 40}

print(s.difference(s1))
🔍 ✅ Membership Operators
s = set("python")

print(s)
print('p' in s)
print('z' not in s)
🚀 🎯 REAL-TIME MINI PROJECT
🛒 E-Commerce Unique Users System

👉 In real applications like Amazon, Flipkart
we should not store duplicate users

users = set()

n = int(input("Enter number of users visiting the site: "))

for i in range(n):
    name = input("Enter user name: ")
    users.add(name)

print("Unique Users:", users)
print("Total Unique Users:", len(users))
