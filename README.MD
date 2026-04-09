📘 Python 30-Day Syllabus

What is Polymorphism?
🎯 DEFINITION

“Polymorphism means one name, multiple forms”

💡 Simple understanding:

👉 Same method name
👉 Different behavior

💡 Real-life example:

👉 Person:

At home → Son
At office → Employee

Same person → different roles

❓ PART 2: Why Polymorphism?

👉 Benefits:

✔ Flexibility
✔ Code reuse
✔ Clean design



“We can use same function for different types of data”

🔥 PART 3: TYPES OF POLYMORPHISM

👉 1) Method Overloading
👉 2) Method Overriding
👉 3) Operator Overloading

🔥 PART 4: METHOD OVERLOADING

👉 Python does NOT support traditional overloading

👉 But we can achieve using default arguments

class Test:
    def add(self, a=None, b=None, c=None):
        if a != None and b != None and c != None:
            print(a + b + c)
        elif a != None and b != None:
            print(a + b)
        else:
            print(a)

t = Test()
t.add(10)
t.add(10, 20)
t.add(10, 20, 30)



“Same method… different behavior”

🔥 PART 5: METHOD OVERRIDING

👉 Child class changes parent method

class Parent:
    def show(self):
        print("Parent method")

class Child(Parent):
    def show(self):
        print("Child method")

c = Child()
c.show()

👉 Output:

👉 Child method


“Child class gives its own implementation”

🔥 PART 6: USING super() IN OVERRIDING
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

🔥 PART 7: OPERATOR OVERLOADING

👉 Same operator → different behavior

print(10 + 20)        # Addition
print("Hello " + "World")  # String concat

👉 Same + operator

👉 Different behavior

🧠 CUSTOM OPERATOR OVERLOADING
class Book:
    def __init__(self, pages):
        self.pages = pages

    def __add__(self, other):
        return self.pages + other.pages

b1 = Book(100)
b2 = Book(200)

print(b1 + b2)

👉 Output:

👉 300

🚀 🎯 REAL-TIME PROJECT 1: PAYMENT SYSTEM
class Payment:
    def pay(self):
        print("Generic payment")

class UPI(Payment):
    def pay(self):
        print("UPI Payment")

class Card(Payment):
    def pay(self):
        print("Card Payment")

for p in [UPI(), Card()]:
    p.pay()

👉 Same method → different outputs

🚀 🎯 REAL-TIME PROJECT 2: NOTIFICATION SYSTEM
class Notification:
    def send(self):
        print("Sending notification")

class Email(Notification):
    def send(self):
        print("Sending Email")

class SMS(Notification):
    def send(self):
        print("Sending SMS")

n = [Email(), SMS()]

for i in n:
    i.send()
🚀 🎯 REAL-TIME PROJECT 3: EMPLOYEE ROLE SYSTEM
class Employee:
    def role(self):
        print("Employee role")

class Developer(Employee):
    def role(self):
        print("Developer coding")

class Manager(Employee):
    def role(self):
        print("Manager managing")

e = [Developer(), Manager()]

for i in e:
    i.role()
Assignment
