📘 Python 30-Day Syllabus

🧠 PART 1: WHAT IS EXCEPTION?
✅ Definition:

In any programming language there are 2 types of errors are possible.
1. Syntax Errors
2. Runtime Errors
1. Syntax Errors:
The errors which occurs because of invalid syntax are called syntax errors.
Eg 1:
x=10
if x==10
print("Hello")
SyntaxError: invalid syntax
Eg 2:
print "Hello"
SyntaxError: Missing parentheses in call to 'print'
Note:
Programmer is responsible to correct these syntax errors. Once all syntax errors are
corrected then only program execution will be started.
2. Runtime Errors:
Also known as exceptions.
While executing the program if something goes wrong because of end user input or
programming logic or memory problems etc then we will get Runtime Errors.


👉 Example:

print(10 / 0)

👉 Output:

❌ ZeroDivisionError

💡 Say:

“This is called runtime error”

❓ WHY EXCEPTION HANDLING?

👉 Without handling:

❌ Program crashes
❌ Bad user experience

👉 With handling:

✔ Smooth execution
✔ Better user experience

🔥 PART 2: TRY – EXCEPT
try:
    a = int(input("Enter number: "))
    print(10 / a)
except:
    print("Error occurred")

💡 Say:

“Try risky code… handle errors in except”

🔥 MULTIPLE EXCEPT BLOCKS
try:
    a = int(input("Enter number: "))
    print(10 / a)
except ZeroDivisionError:
    print("Cannot divide by zero")
except ValueError:
    print("Invalid input")
🔥 PART 3: ELSE BLOCK
try:
    a = int(input("Enter number: "))
except ValueError:
    print("Invalid input")
else:
    print("You entered:", a)

👉 Runs only if no exception

🔥 PART 4: FINALLY BLOCK
try:
    print("Try block")
except:
    print("Except block")
finally:
    print("Always executes")

👉 Always runs

🔥 PART 5: CUSTOM EXCEPTION
class MyError(Exception):
    pass

try:
    raise MyError("Custom error occurred")
except MyError as e:
    print(e)
🚀 🎯 REAL-TIME PROJECT 1: ATM SYSTEM
balance = 1000

try:
    amount = int(input("Enter amount: "))
    if amount > balance:
        raise Exception("Insufficient balance")
    balance -= amount
    print("Withdraw successful")
except ValueError:
    print("Invalid input")
except Exception as e:
    print(e)
🧠 PART 6: FILE HANDLING
✅ Definition:

“File handling is used to read and write data from files”

🔥 OPEN FILE
f = open("test.txt", "w")
f.write("Hello Python")
f.close()
🔥 READ FILE
f = open("test.txt", "r")
print(f.read())
f.close()
🔥 APPEND MODE
f = open("test.txt", "a")
f.write("\nNew Line Added")
f.close()
🔥 BEST PRACTICE (WITH)
with open("test.txt", "r") as f:
    print(f.read())

👉 No need to close manually

🚀 🎯 REAL-TIME PROJECT 2: FILE LOGGER SYSTEM
try:
    with open("data.txt", "a") as f:
        name = input("Enter name: ")
        f.write(name + "\n")
        print("Saved successfully")
except Exception as e:
    print("Error:", e)
🚀 🎯 REAL-TIME PROJECT 3: SAFE FILE READER
try:
    with open("sample.txt", "r") as f:
        print(f.read())
except FileNotFoundError:
    print("File not found")
😂 FUN LINE

“Errors will come…
but smart developers handle them 😄🔥”

🧠 ADVANCED INSIGHT

👉 Used in:

✔ Banking apps
✔ Logging systems
✔ File processing
✔ APIs

🎯 ENDING

Today we learned:

✔ Exception Handling
✔ try-except-else-finally
✔ Custom exceptions
✔ File handling
✔ Real-world projects

Assignment
