📘 Python 30-Day Syllabus

# Day 16 - Object Oriented Programming (OOPs) Part 01

## 📚 Topics Covered So Far

1. Fundamentals of Python  
2. Operators  
3. Input Function  
4. Flow Control  
5. String Data Type  
6. List Data Type  
7. Tuple  
8. Set  
9. Dictionary  
10. Functions  
11. Modules  
12. Packages  

---

## 🚀 Advanced Python Topics

13. OOPs  
14. Exception Handling  
15. File Handling  
16. Serialization  
17. Regular Expressions (RE)  
18. Multithreading  
19. PDB (Python Debugger)  
20. Decorators  
21. NumPy, Pandas  

---

# 🧠 OOPs Concepts

## 📌 Class

- In Python, everything is an object.
- A **class** is a blueprint or model used to create objects.
- A class contains:
  - Variables (data)
  - Methods (functions)

### Syntax:
```python
class ClassName:
    """Doc String"""
    body
Example:
class Student:
    """This is Student class with required data"""

print(Student.__doc__)
help(Student)
📌 Object
An object is the physical existence of a class.
We can create multiple objects for a class.
Example:
s = Student()
📌 Reference Variable
A variable that refers to an object is called a reference variable.
📌 Example Program
class Student:
    def __init__(self, name, rollno, marks):
        self.name = name
        self.rollno = rollno
        self.marks = marks

    def talk(self):
        print("Hello My Name is", self.name)
        print("My Rollno is", self.rollno)
        print("My marks are:", self.marks)

s = Student("venky", 102, 80)
s.talk()
📌 self Variable
self represents the current object.
It is used to access instance variables and methods.
📌 Constructor
A constructor is a special method.
It is automatically executed when an object is created.
Syntax:
def __init__(self):
📌 Types of Variables
1️⃣ Instance Variables
Defined inside constructor using self
Access methods:
Inside class → using self
Outside class → using object reference
2️⃣ Static Variables
Shared among all objects
Defined inside class but outside methods
Example:
class Test:
    x = 10  # static variable

    def __init__(self):
        self.y = 20  # instance variable

t1 = Test()
t2 = Test()

print("t1:", t1.x, t1.y)
print("t2:", t2.x, t2.y)
3️⃣ Local Variables
Defined inside methods
Accessible only within that method
Example:
class Test:
    def m1(self):
        a = 100
        print(a)

    def m2(self):
        b = 200
        print(b)

t = Test()
t.m1()
t.m2()
📌 Types of Methods
1️⃣ Instance Methods
Use self
Access instance variables
class Student:
    def __init__(self, name, rollno, marks):
        self.name = name
        self.rollno = rollno
        self.marks = marks

    def talk(self):
        print(self.name, self.rollno, self.marks)
2️⃣ Class Methods
Use @classmethod decorator
Use cls instead of self
Access class (static) variables
class Animal:
    legs = 4

    @classmethod
    def walk(cls, name):
        print(f"{name} walks with {cls.legs} legs")

Animal.walk("Dog")
3️⃣ Static Methods
Use @staticmethod decorator
No self or cls
Used for utility functions
class VenkatMath:
    @staticmethod
    def add(x, y):
        print("Sum:", x + y)

    @staticmethod
    def product(x, y):
        print("Product:", x * y)

VenkatMath.add(10, 20)
VenkatMath.product(10, 20)
📌 Important Note
Mostly used methods:
Instance Methods ✅
Static Methods ✅
Class methods are rarely used.

---

# 🎯 YouTube / Upload Details

## 🏷️ Title:
**Python OOPs Tutorial Part 1 | Classes, Objects, Methods Explained in Telugu**

---

## 📝 Description:

In this video, we learn Object Oriented Programming (OOPs) concepts in Python from basics.

Topics Covered:

What is Class and Object
Reference Variable
Constructor (init)
Instance Variables
Static Variables
Local Variables
Types of Methods
Instance Method
Class Method
Static Method

This is Part 1 of OOPs series.

Perfect for beginners who want to master Python step by step.

Assignment
