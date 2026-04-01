📘 Python 30-Day Syllabus

📘 🚀 DAY 10 – DICTIONARIES (REFINED NOTES)
🧠 ✅ What is Dictionary?

👉 If we want to represent a group of objects as key-value pairs, then we use Dictionary

🎯 💡 Real-Time Examples
Roll Number → Name
Phone Number → Address
IP Address → Domain Name

👉 In other languages, Dictionary is called Map

🛠️ ✅ How to Create Dictionary
d = {}
d = dict()

d[100] = "python"
d[200] = "AI"

print(d)
🔹 Predefined Data
d = {100: "python", 200: "AI"}
🔍 ✅ Accessing Data
d = {100: "python", 200: "AI"}

print(d[100])
print(d[200])
❗ KeyError Example
print(d[300])   # KeyError ❌
🔄 ✅ Updating Dictionary
d = {100: "python", 200: "AI"}

d[300] = "ML"     # Add new
d[100] = "ML"     # Update existing

print(d)
❌ ✅ Deleting Elements
d = {100: "python", 200: "AI"}

del d[100]
print(d)
🔹 clear()
d = {100: "python", 200: "AI"}

d.clear()
print(d)
🧠 ✅ Important Functions
🔹 len()
d = {100: "python", 200: "AI"}
print(len(d))
🔹 get()
print(d.get(100))

👉 Safe way (no error)

🔹 keys()
print(d.keys())
🔹 values()
print(d.values())
🔹 items()
print(d.items())
🔁 Looping Dictionary
for k, v in d.items():
    print(k, "--", v)
🚀 🎯 PROGRAM 1
👉 Sum of Values
d = eval(input("Enter dictionary: "))
s = sum(d.values())

print("Sum =", s)
🚀 🎯 PROGRAM 2
👉 Count Characters in String
word = input("Enter any word: ")

d = {}

for x in word:
    d[x] = d.get(x, 0) + 1

for k, v in d.items():
    print(k, "occurred", v, "times")

👉 💡 Example:

Input: pythonyy
Output:
p 1
y 3
t 1
h 1
o 1
n 1
