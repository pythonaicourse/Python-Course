📘 Python 30-Day Syllabus

# 🧠 **Day 19 – OOPs Part 04 (Advanced Concepts)**

## Abstract Class | Interface | Access Modifiers | Mini Application

---

# 🔷 1) ABSTRACT METHOD

---

## ✅ Definition:

An **abstract method** is a method that is **declared but does not contain implementation**.

👉 It only defines *what to do*, not *how to do*

---

## ✅ Syntax:

```python
from abc import ABC, abstractmethod

class Test(ABC):
    @abstractmethod
    def m1(self):
        pass
```

---

## 💡 Important Points:

* Must be inside an abstract class
* Child class **must implement** it
* Cannot create object if not implemented

---

# 🔷 2) ABSTRACT CLASS

---

## ✅ Definition:

An **abstract class** is a class that contains **at least one abstract method**.

---

## 💡 Key Points:

* Cannot create object
* Used as a blueprint
* Child classes must implement abstract methods

---

## ✅ Example:

```python
from abc import ABC, abstractmethod

class Test(ABC):
    @abstractmethod
    def m1(self):
        pass

# t = Test() ❌ Error (cannot create object)
```

---

# 🔷 3) INTERFACE (Python Concept)

---

## ✅ Definition:

An **interface** is a class that contains **only abstract methods**.

👉 It acts like a contract
👉 Forces child classes to implement methods

---

## ✅ Example:

```python
from abc import ABC, abstractmethod

class DBInterface(ABC):
    @abstractmethod
    def connect(self):
        pass

    @abstractmethod
    def disconnect(self):
        pass


class Oracle(DBInterface):
    def connect(self):
        print("Connecting to Oracle Database")

    def disconnect(self):
        print("Disconnecting from Oracle Database")


class Sybase(DBInterface):
    def connect(self):
        print("Connecting to Sybase Database")

    def disconnect(self):
        print("Disconnecting from Sybase Database")


dbname = input("Enter Database Name (Oracle/Sybase): ")

if dbname == "Oracle":
    obj = Oracle()
elif dbname == "Sybase":
    obj = Sybase()
else:
    print("Invalid database")
    exit()

obj.connect()
obj.disconnect()
```

---

# 🔷 4) DIFFERENCE

## Concrete Class vs Abstract Class vs Interface

| Feature         | Concrete Class | Abstract Class      | Interface        |
| --------------- | -------------- | ------------------- | ---------------- |
| Methods         | Normal methods | Abstract + normal   | Only abstract    |
| Object Creation | Yes            | No                  | No               |
| Purpose         | Implementation | Partial abstraction | Full abstraction |

---

# 🔷 5) ACCESS MODIFIERS

---

## ✅ 1) Public Variable

👉 Accessible everywhere

```python
name = "Venky"
```

---

## ✅ 2) Protected Variable (_)

👉 Internal use (convention only)

```python
_name = "Venky"
```

---

## ✅ 3) Private Variable (__)

👉 Cannot access directly outside class

```python
__name = "Venky"
```

---

## 💡 Example:

```python
class Test:
    x = 10        # public
    _y = 20       # protected
    __z = 30      # private

    def m1(self):
        print(self.x)
        print(self._y)
        print(self.__z)

t = Test()
t.m1()

print(Test.x)
print(Test._y)

# print(Test.__z) ❌ Error
print(Test._Test__z)  # Access using name mangling
```

---

# 🔷 6) MINI BANK APPLICATION (REAL-TIME)

---

## 🎯 Concept:

Using Abstract Class + Interface + Access Modifier

---

```python
from abc import ABC, abstractmethod

class Bank(ABC):
    def __init__(self, name, balance):
        self.name = name
        self._balance = balance   # protected

    @abstractmethod
    def interest(self):
        pass


class SavingsAccount(Bank):
    def interest(self):
        print(self.name, "Savings Interest:", self._balance * 0.05)


class CurrentAccount(Bank):
    def interest(self):
        print(self.name, "No interest for current account")


acc1 = SavingsAccount("Rahul", 10000)
acc1.interest()

acc2 = CurrentAccount("Ravi", 20000)
acc2.interest()
```

---

# 😂 FUN UNDERSTANDING

👉 Abstract Class = Rule Book 📜
👉 Interface = Strict Contract 🤝
👉 Child Class = Implementation 👨‍💻

---

# 🎯 SUMMARY

---

✔ Abstract Method → only declaration
✔ Abstract Class → cannot create object
✔ Interface → only abstract methods
✔ Access Modifiers → control data access
✔ Used in real-world applications

---

# 🚀 FINAL LINE 

“Advanced OOP concepts are not just theory…
they are used in real-world systems like banking, APIs, and large applications 🔥”


Assignment
