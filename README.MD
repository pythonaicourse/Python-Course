📘 Python 30-Day Syllabus

📘 🚀 FLOW CONTROL STATEMENTS (FULL NOTES + SCRIPT STYLE)
🧠 🎯 1. What is Flow Control? (SUPER DEFINITION)

👉 Flow Control Statements control the execution flow of a program.

👉 In simple words:

💡
“Flow control decides which statement to execute, when to execute, and how many times to execute”



👉 “Flow control is the brain of any program 🧠”

🎯 🔥 TYPES OF FLOW CONTROL
Conditional Statements (Decision Making)
Looping Statements (Iteration)
Control Statements (break, continue, pass)
🧠 🚦 2. CONDITIONAL STATEMENTS
✅ SUPER DEFINITION

👉 Used to execute code based on condition

💻 Example:
age = 18

if age >= 18:
    print("Eligible to vote")
🎯 REAL-TIME EXAMPLES

👉 Voting system
👉 Login system
👉 Exam result

💥 Example: Exam Result
marks = 75

if marks >= 50:
    print("Pass")
else:
    print("Fail")

👉 💡 Say:

“Every decision in real life → uses conditions”

🔁 🔄 3. LOOPING STATEMENTS
✅ SUPER DEFINITION

👉 Used to repeat a block of code multiple times

💻 Example:
for i in range(5):
    print("Hello")
🎯 REAL-TIME EXAMPLES

👉 ATM retries
👉 Mobile notifications
👉 Daily tasks

💥 Example: OTP System
for i in range(3):
    otp = input("Enter OTP: ")
    if otp == "1234":
        print("Verified")
        break

👉 💡 Say:

“Loop means repetition until condition is satisfied”

🧠 🛑 4. CONTROL STATEMENTS
🔹 break

👉 Stops the loop immediately

for i in range(10):
    if i == 5:
        break
    print(i)
🎯 REAL-TIME

👉 Stop login attempts
👉 Stop game when user wins

🔹 continue

👉 Skips current iteration

for i in range(5):
    if i == 2:
        continue
    print(i)
🎯 REAL-TIME

👉 Skip invalid data
👉 Skip blocked users

🔹 pass

👉 Does nothing (placeholder)

for i in range(5):
    pass
🎯 REAL-TIME

👉 Future code placeholder
👉 Empty logic block

🔥 🎯 REAL-TIME MINI PROJECTS
🚀 💳 PROJECT 1: ATM PIN SYSTEM
correct_pin = "1234"

for i in range(3):
    pin = input("Enter PIN: ")
    
    if pin == correct_pin:
        print("Access Granted ✅")
        break
    else:
        print("Wrong PIN ❌")

else:
    print("Card Blocked 🔒")
🚀 🎮 PROJECT 2: GAME LOOP
while True:
    choice = input("Play game? (yes/no): ")
    
    if choice == "no":
        break
    print("Game running 🎮")
🚀 🛒 PROJECT 3: BILLING SYSTEM
total = 0

while True:
    price = input("Enter price (or stop): ")
    
    if price == "stop":
        break
    
    total += int(price)

print("Total Bill:", total)
🎯 🧠 SUMMARY (ENDING)

👉 Flow Control includes:

✔ Conditions → Decision making
✔ Loops → Repetition
✔ Control statements → Manage flow

🔥 FINAL POWER Full LINE



“Without flow control, program is just lines of code…
With flow control, program becomes intelligent 🔥

Assignment
