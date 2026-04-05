📘 Python 30-Day Syllabus

🧠 PART 1: What is a Module?

👉 Definition:

“A module is a Python file that contains functions, variables, or classes”

💡 Simple Explanation:

“One Python file = one module”

👉 Example:

If you create a file called:

👉 calculator.py

That file itself is a module.

❓ PART 2: Why Modules?

👉 Without modules:

Everything in one file
Code becomes messy
Difficult to manage

👉 With modules:

✔ Clean code
✔ Reusable functions
✔ Easy maintenance



“In real projects, code is always divided into multiple files”

🔥 PART 3: Creating a Module

👉 Step 1: Create a file → mymath.py

def add(a, b):
    return a + b

def sub(a, b):
    return a - b
🔗 PART 4: Using a Module (import)

👉 Create another file → main.py

import mymath

print(mymath.add(10, 20))
print(mymath.sub(30, 10))


“We import the module and use its functions”

🔥 PART 5: from...import
from mymath import add

print(add(5, 3))

👉 Advantage:

“No need to write module name every time”

🔥 PART 6: Import with Alias
import mymath as m

print(m.add(10, 5))



“We can use a short name for convenience”

🚀 🎯 REAL-TIME PROJECT 1: CALCULATOR SYSTEM

👉 File: calculator.py

def add(a, b):
    return a + b

def multiply(a, b):
    return a * b

👉 File: main.py

import calculator

print("Addition:", calculator.add(10, 20))
print("Multiplication:", calculator.multiply(5, 5))

👉 Real-world idea:

“Different functionalities are stored in separate files”

🚀 🎯 REAL-TIME PROJECT 2: LOGIN SYSTEM

👉 File: auth.py

def login(user, password):
    if user == "admin" and password == "1234":
        return "Login Successful"
    else:
        return "Login Failed"

👉 File: app.py

import auth

print(auth.login("admin", "1234"))

👉 Real-world idea:

“Authentication logic is separated into its own module”

🚀 🎯 REAL-TIME PROJECT 3: UTILITY FUNCTIONS

👉 File: utils.py

def greet(name):
    return "Hello " + name

def square(n):
    return n * n

👉 File: main.py

from utils import greet, square

print(greet("Rahul"))
print(square(4))

👉 Real-world idea:

“Common reusable functions are stored in utility modules”

😂 FUN LINE

“Modules are like a team…
Each file handles one responsibility”

🧠 IMPORTANT POINTS

✔ One file = one module
✔ Use import to access module
✔ Use from...import for direct access
✔ Use alias for simplicity

Assignment
