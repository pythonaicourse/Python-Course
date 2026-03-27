📘 Python 30-Day Syllabus

🚀 DAY 08 – TUPLES (NOTES)
🧠 ✅ 1. What is Tuple?

👉 A tuple is a collection of multiple values stored in a single variable.

👉 It is ordered and immutable (cannot be changed)

💻 Example:
data = (10, 20, 30)
🎯 ✅ 2. Where we can use Tuple?

👉 Use tuples when data should NOT change:

Bank Account Number
Date of Birth
Aadhaar / ID
Coordinates (location)
Fixed configuration values

👉 💡 Line to say:

“Whenever data should be secure and constant → use tuple 🔒”

⚔️ ✅ 3. Difference: List vs Tuple
Feature	List	Tuple
Syntax	[ ]	( )
Mutable	✅ Yes	❌ No
Performance	Slower	Faster
Use Case	Changeable data	Fixed data

👉 💡 Simple line:

“List is flexible… Tuple is fixed 🔒”

🔄 ✅ 4. Mutable vs Immutable
🔹 Mutable:

👉 Data can be changed

Example:

list_data = [10, 20]
list_data[0] = 99
🔹 Immutable:

👉 Data cannot be changed

Example:

tuple_data = (10, 20)
tuple_data[0] = 99   # Error ❌

👉 💡 Line to say:

“Immutable means Python protects the data from modification”

🔢 ✅ 5. Accessing Tuple Elements

👉 Same as list (indexing)

data = ("Rahul", 25, "India")

print(data[0])   # Rahul
print(data[-1])  # India

👉 Slicing also works:

print(data[0:2])
🚀 🎯 MINI PROJECTS
🧾 🔥 Project 1: User Profile System
user_profile = ("Rahul", 25, "rahul@gmail.com", "India")

print("User Profile:", user_profile)

print("Name:", user_profile[0])
print("Age:", user_profile[1])
print("Email:", user_profile[2])
print("Country:", user_profile[3])
🏦 🔥 Project 2: Bank Account Details
account = (1234567890, "Rahul", "Savings", 25000.50)

print("Account Number:", account[0])
print("Name:", account[1])
print("Type:", account[2])
print("Balance:", account[3])

👉 💡 Explain:

“In real systems, account number should not change…
So tuple is used 🔒”

🎯 🎬 YOUTUBE SETUP
