📘 Python 30-Day Syllabus

📘 🚀 DAY 11 – FUNCTIONS 

❌ 🔁 Before Functions (Problem)
a = 10
b = 20
print("The sum", a+b)
print("The difference", a-b)
print("The product", a*b)

a = 300
b = 400
print("The sum", a+b)
print("The difference", a-b)
print("The product", a*b)

👉 ❗ Problem:

Code repetition
Difficult to maintain
Not efficient
🧠 ✅ What is a Function?

👉 If a group of statements is repeatedly required,
instead of writing them again and again,
we define them as a single unit (function) and reuse it.

🎯 💡 Types of Functions
Built-in Functions
User-defined Functions
🔹 1. Built-in Functions

Examples:

id()
type()
input()
eval()
🔹 2. User-defined Functions
🛠️ ✅ Function Syntax
def function_name(parameters):
    """doc string"""
    # Business logic
    return value
🔧 ✅ How to Create and Call Function
def function_name(parameter):
    # Business logic
    print(parameter)

function_name("Python")
🎯 ✅ Simple Program
def first_program():
    print("Hello")

first_program()
📥 ✅ Parameters Example
def wish(name):
    print("Hello", name, "Good Evening")

wish("Python")
🔁 ✅ Return Statement

👉 A function can take input, process it, and return output using return

🎯 Program 1: Addition
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
🎯 Program 2: Even or Odd
def even_odd(num):
    if num % 2 == 0:
        print(num, "is Even")
    else:
        print(num, "is Odd")

even_odd(10)
🔄 ✅ Returning Multiple Values
def operations(a, b):
    return a + b, a - b, a * b

result = operations(10, 20)
print(result)
📌 ✅ Types of Arguments

👉 There are 4 types:

Positional Arguments
Keyword Arguments
Default Arguments
Variable Length Arguments
🔹 1. Positional Arguments

👉 Arguments are passed in correct order

def sub(a, b):
    print(a - b)

sub(10, 20)
sub(20, 10)
🔹 2. Keyword Arguments

👉 Arguments are passed using parameter names

def wish(name, msg):
    print("Hello", name, msg)

wish(name="Venky", msg="Good Evening")
wish(msg="Good Evening", name="Venky")

Assignment
