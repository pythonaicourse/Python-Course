📘 Python 30-Day Syllabus

# 📘 Python Learning Series – Day 04

## 🚀 Core Concepts of Python Programming

In today’s session, we covered the **fundamental building blocks of Python**:

- Identifiers  
- Reserved Words (Keywords)  
- Data Types  
- Number Systems  

---

## 💡 Part 1: Identifiers

An **identifier** is the name given to a variable, function, class, or module.

### 📌 Example
```python
a = 10  # 'a' is an identifier
✅ Rules for Identifiers
Allowed characters:
Alphabets (a-z, A-Z)
Digits (0-9)
Underscore (_)
Cannot start with a digit ❌
123abc → Invalid
Case-sensitive
total ≠ TOTAL
Special symbols not allowed ❌
$, @, #
Cannot use reserved words ❌
def, if
✔ Valid Identifiers
total123
_value
❌ Invalid Identifiers
123total
ca$h
def

💡 Tip:
Identifiers starting with _ indicate private usage.

💡 Part 2: Reserved Words (Keywords)

Reserved words are predefined words in Python with special meaning.

📌 Examples
True, False, None
if, else, elif
for, while, break
def, class, return
🔍 View all keywords in Python
import keyword
print(keyword.kwlist)
⚠️ Important

You cannot use keywords as identifiers

def = 10  # ❌ Error
💡 Part 3: Data Types

A data type represents the type of value stored in a variable.

Python is a dynamically typed language, so no need to declare types explicitly.

📌 Examples
a = 10       # int
b = 10.5     # float
c = "hello"  # string
📊 Common Data Types
int → Integer values (10, 20)
float → Decimal values (10.5)
complex → (3+5j)
bool → True / False
str → Strings
list, tuple, set, dict
💡 Special Functions
type() → Returns data type
id() → Returns memory address
print() → Displays output
💡 Part 4: Number Systems

Python supports multiple number formats:

Type	Example
Decimal	10
Binary	0b1010
Octal	0o12
Hexadecimal	0xA
📌 Example
print(0b10)  # 2
print(0o10)  # 8
print(0x10)  # 16
🎯 Summary
Identifiers follow strict naming rules
Reserved words cannot be used as variable names
Python automatically assigns data types
Multiple number systems are supported
📅 Day 04 Completed ✅

Stay tuned for Day 05 where we will explore more concepts with practical examples!
