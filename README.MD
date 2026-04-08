📘 Python 30-Day Syllabus

🧠 PART 1: What is Inheritance?

👉 Definition:

“Inheritance allows one class to acquire properties and methods of another class”

💡 Simple understanding:

👉 Parent → Child

Child can use parent features

💡 Real-life example:

👉 Father → Child

Child inherits properties

❓ PART 2: Why Inheritance?

👉 Without inheritance:

Code repetition ❌
Hard to maintain ❌

👉 With inheritance:

✔ Code reuse
✔ Clean structure
✔ Easy maintenance

💡 Powerful line:

“Don’t repeat code… reuse it 🔥”

🔥 PART 3: Basic Example
class Parent:
    def property(self):
        print("This is parent property")

class Child(Parent):
    pass

c = Child()
c.property()

👉 Say:

“Child class can directly use parent methods”

🔥 PART 4: Adding Child Features
class Parent:
    def show(self):
        print("Parent method")

class Child(Parent):
    def display(self):
        print("Child method")

c = Child()
c.show()
c.display()

🧠 PART 5: TYPES OF INHERITANCE
1️⃣ Single Inheritance

👉 One parent → One child

class A:
    def method1(self):
        print("A class")

class B(A):
    def method2(self):
        print("B class")
2️⃣ Multilevel Inheritance

👉 Grandparent → Parent → Child

class A:
    def method1(self):
        print("A")

class B(A):
    def method2(self):
        print("B")

class C(B):
    def method3(self):
        print("C")
3️⃣ Multiple Inheritance

👉 One child → multiple parents

class A:
    def m1(self):
        print("A")

class B:
    def m2(self):
        print("B")

class C(A, B):
    pass
4️⃣ Hierarchical Inheritance

👉 One parent → multiple children

class A:
    def show(self):
        print("A")

class B(A):
    pass

class C(A):
    pass
5️⃣ Hybrid Inheritance

👉 Combination of multiple types



“Combination of all inheritance types”

🚀 🎯 REAL-TIME PROJECT 1: VEHICLE SYSTEM
class Vehicle:
    def start(self):
        print("Vehicle started")

class Car(Vehicle):
    def drive(self):
        print("Car driving")

c = Car()
c.start()
c.drive()
🚀 🎯 REAL-TIME PROJECT 2: EMPLOYEE SYSTEM
class Employee:
    def __init__(self, name):
        self.name = name

class Developer(Employee):
    def work(self):
        print(self.name, "is coding")

d = Developer("Rahul")
d.work()
🚀 🎯 REAL-TIME PROJECT 3: ONLINE PLATFORM
class User:
    def login(self):
        print("User login")

class Admin(User):
    def manage(self):
        print("Admin managing system")

a = Admin()
a.login()
a.manage()
😂 FUN LINE

“Inheritance is like family property…
You don’t create it again, you inherit it 😄”

🧠 ADVANCED POINT

👉 Inheritance helps in:

✔ Code reuse
✔ Extensibility
✔ Maintainable architecture
Assignment

🧠 PART 6: MRO (Method Resolution Order)
🎯 SUPER DEFINITION

👉 “MRO defines the order in which Python searches for methods in inheritance”

💡 Simple line:

“When you call a method… Python checks classes in a specific order 🔥”

❓ WHY MRO IS IMPORTANT

👉 In multiple inheritance:

Same method name in multiple classes 😳
Which method should run?

👉 Answer → MRO

🔥 BASIC EXAMPLE
class A:
    def show(self):
        print("A class")

class B(A):
    pass

class C(B):
    pass

c = C()
c.show()

👉 Flow:

C → B → A

🔥 MULTIPLE INHERITANCE EXAMPLE
class A:
    def show(self):
        print("A class")

class B:
    def show(self):
        print("B class")

class C(A, B):
    pass

c = C()
c.show()

👉 Output:

👉 A class

👉 Why?

👉 MRO follows:

👉 Left → Right order

🧠 CHECK MRO ORDER
print(C.mro())

👉 Output shows:

👉 C → A → B → object



“This is the path Python follows to find methods”

🚀 🎯 REAL-TIME EXAMPLE (MRO)

👉 Scenario:

Multiple features in app

class Login:
    def action(self):
        print("Login feature")

class Payment:
    def action(self):
        print("Payment feature")

class App(Login, Payment):
    pass

a = App()
a.action()

👉 Output:

👉 Login feature

👉 Because MRO → Login first

🔥 🧠 PART 7: super() METHOD
🎯 SUPER DEFINITION

👉 “super() is used to call parent class methods”

💡 Simple line:

“Child can access parent using super() 🔥”

🔥 BASIC EXAMPLE
class Parent:
    def show(self):
        print("Parent method")

class Child(Parent):
    def show(self):
        super().show()
        print("Child method")

c = Child()
c.show()

👉 Output:

Parent method
Child method

🧠 WHY super()?

👉 To reuse parent code
👉 Avoid duplication

🔥 CONSTRUCTOR WITH super()
class Parent:
    def __init__(self):
        print("Parent constructor")

class Child(Parent):
    def __init__(self):
        super().__init__()
        print("Child constructor")

c = Child()

👉 Output:

Parent constructor
Child constructor

🚀 🎯 REAL-TIME PROJECT (super())

👉 Scenario: Employee system

class Employee:
    def __init__(self, name):
        self.name = name

class Developer(Employee):
    def __init__(self, name, skill):
        super().__init__(name)
        self.skill = skill

    def show(self):
        print(self.name, "is a", self.skill, "developer")

d = Developer("Rahul", "Python")
d.show()

👉 Output:

Rahul is a Python developer

💡 Real-world:

👉 Parent → common data
👉 Child → extra features

😂 FUN LINE

“MRO decides WHO to call 😄
super() decides HOW to call 🔥”

🧠 ADVANCED INSIGHT

👉 MRO uses:

👉 C3 Linearization algorithm


