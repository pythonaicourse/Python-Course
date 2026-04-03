📘 Python 30-Day Syllabus

📘 🚀 DAY 12 – FUNCTIONS (PART 02) NOTES
🧠 ✅ Types of Arguments
Positional Arguments
Keyword Arguments
Default Arguments
Variable Length Arguments
🔹 ✅ 3. Default Arguments

👉 Sometimes we can provide default values to function parameters.

👉 If the user does not pass a value, default will be used.

💻 Example:
def wish(name="Guest"):
    print("Hello", name, "Welcome to this site")

wish("Venky")
wish()

👉 💡 Output:

Hello Venky Welcome to this site
Hello Guest Welcome to this site
🎯 Real-Time Example

👉 Login system:

def login(user="Guest"):
    print("Welcome", user)

login("Rahul")
login()

👉 💡 Use Case:

Default user login
Optional inputs
🔹 ✅ *4. Variable Length Arguments (args)

👉 Sometimes we don’t know how many inputs user will give
👉 We use *args

💻 Example:
def total_sum(*n):
    total = 0
    for n1 in n:
        total = total + n1
    print("The sum =", total)

total_sum()
total_sum(10)
total_sum(10, 20)
total_sum(10, 20, 30)
🎯 Real-Time Example

👉 Shopping Cart:

def cart_total(*prices):
    print("Total Bill:", sum(prices))

cart_total(100, 200, 300)

👉 💡 Use Case:

E-commerce billing
Dynamic inputs
🌍 ✅ Types of Variables
Local Variables
Global Variables
🔹 ✅ Global Variables

👉 Variables declared outside the function

a = 10

def f1():
    print(a)

def f2():
    print(a)

f1()
f2()

👉 💡 Use Case:

Configuration values
Shared data
🔹 ✅ Local Variables

👉 Variables declared inside a function

def f1():
    a = 10
    print(a)

f1()

👉 💡 Important:

Local variables cannot be accessed outside the function
🔁 ✅ Recursive Functions

👉 A function that calls itself is called recursion

💻 Example: Factorial
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))

👉 💡 Real-Time Example:

Calculations
Tree structures
AI algorithms
⚡ ✅ Anonymous (Lambda) Functions

👉 Functions without name

🔹 Normal Function
def square(n):
    return n * n
🔹 Lambda Function
s = lambda n: n * n
print("The square of 4 is:", s(4))
🎯 Real-Time Example
numbers = [1, 2, 3, 4]

squares = list(map(lambda x: x*x, numbers))
print(squares)

👉 💡 Use Case:

Short operations
Data processing
🎯 🧠 FINAL SUMMARY

✔ Default Arguments → Default values
✔ *args → Multiple inputs
✔ Local vs Global variables
✔ Recursion → Function calling itself
✔ Lambda → Short functions
