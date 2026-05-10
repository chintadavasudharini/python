# Python OOP Essentials 🚀

> Professional Object-Oriented Programming notes in Python with real-world examples, outputs, memory visualization, and interview-focused explanations.

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![OOP](https://img.shields.io/badge/OOP-Concepts-green?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)

---

# 📖 Table of Contents

- Introduction to OOP
- Class in Python
- Object in Python
- `pass` Statement
- Constructor `__init__()`
- Default Parameters
- Multiple Parameters
- Methods in Classes
- Understanding `self`
- Class vs Instance Variables
- Real-World Bank Account Project
- Memory Visualization
- Important OOP Concepts

---

# 🚀 Introduction to OOP

Python is an Object-Oriented Programming language that helps developers build:

- Scalable applications
- Reusable components
- Secure systems
- Real-world models

## ✅ Advantages of OOP

- Code Reusability
- Better Maintainability
- Scalability
- Modular Development
- Real-world Modeling
- Encapsulation & Data Security

---

# 1️⃣ Class in Python

A **Class** is a blueprint used to create objects.

## Example

```python
class Student:
    name = "Vasudha"
    age = 23

print(Student.name)
print(Student.age)
```

## Output

```python
Vasudha
23
```

---

# 2️⃣ Object in Python

An **Object** is a real instance created from a class.

## Example

```python
class Student:
    name = "Vasudha"
    age = 23

s1 = Student()

print(s1.name)
print(s1.age)
```

## Output

```python
Vasudha
23
```

---

# 3️⃣ Empty Class using `pass`

Python classes cannot be empty.

## Example

```python
class Person:
    pass
```

---

# 4️⃣ Constructor — `__init__()`

The `__init__()` method is automatically executed when an object is created.

## Example

```python
class Person:

    def __init__(self, name, age):
        self.name = name
        self.age = age

p1 = Person("Vasu", 23)

print(p1.name)
print(p1.age)
```

## Output

```python
Vasu
23
```

---

# 🔥 Internal Working

When object is created:

```python
p1 = Person("Vasu", 23)
```

Python internally calls:

```python
__init__(p1, "Vasu", 23)
```

---

# 5️⃣ Default Parameters in Constructor

## Example

```python
class Person:

    def __init__(self, name, age=18):
        self.name = name
        self.age = age

p1 = Person("Vasu")
p2 = Person("Vasudharini", 23)

print(p1.name, p1.age)
print(p2.name, p2.age)
```

## Output

```python
Vasu 18
Vasudharini 23
```

---

# 6️⃣ Multiple Parameters

## Example

```python
class Person:

    def __init__(self, name, age, city, country):
        self.name = name
        self.age = age
        self.city = city
        self.country = country

p1 = Person("Vasu", 23, "Vijayawada", "India")

print(p1.name)
print(p1.age)
print(p1.city)
print(p1.country)
```

## Output

```python
Vasu
23
Vijayawada
India
```

---

# 7️⃣ Methods in Python Classes

Methods are functions defined inside a class.

## Example

```python
class Student:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("Name:", self.name)
        print("Age:", self.age)

s1 = Student("Vasudha", 23)

s1.display()
```

## Output

```python
Name: Vasudha
Age: 23
```

---

# 8️⃣ Slove Some Examples

---

# 🐶 1. Dog Class Example

## 📝 Question

Create a class called `Dog`

- Add an `__init__` method with parameters `name` and `age`
- Store them as properties using `self`
- Add a method called `bark`
- Print the dog's name followed by `" says Woof!"`
- Create an object `d1`
- Call the `bark()` method

---

# 👤 2. Person Class Example

## 📝 Question

Create a class called `Person`

- Add an `__init__` method that takes `name` and `age`
- Add a method called `greet`
- Print `"Hello, my name is"` followed by the name
- Create an object `p1`
- Call the `greet()` method

---

# 🚗 3.Car Class Example

A simple Python OOP example demonstrating how to create a class, constructor, object, and method.

---

# 📝 Question

Create a class called `Car`

- Add an `__init__` method with a `brand` parameter
- Store the brand as a property using `self`
- Add a method called `show`
- Print the brand name
- Create an object `c1` with brand `"Ford"`
- Call the `show()` method

---

# 9️⃣ Understanding `self`

`self` refers to the current object instance.

It is used to:

- Access object variables
- Access methods
- Link methods to objects

---

## Example

```python
class Person:

    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print(f"Hello, my name is {self.name}")

p1 = Person("Vasu", 23)

p1.greet()
```

## Output

```python
Hello, my name is Vasu
```

---

# 🔥 Internal Method Call

When:

```python
p1.greet()
```

Python internally converts it into:

```python
Person.greet(p1)
```

---

# 🔟 Class Variables vs Instance Variables

## Example

```python
class Person:

    lastname = "Ch"

    def __init__(self, name):
        self.name = name

    def show_name(self):
        print(f"Hello, I'm {self.name} {self.lastname}")

p1 = Person("Vasu")
p2 = Person("Vasudha")

print(p1.lastname)
print(p2.lastname)

p1.show_name()
```

## Output

```python
Ch
Ch
Hello, I'm Vasu Ch
```

---

# 🏦 Real-World Project — Bank Account System

## Complete Code

```python
class BankAccount:

    # Constructor
    def __init__(self, name, balance):
        self.name = name
        self.balance = balance

    # Deposit Method
    def deposit(self, amount):
        self.balance += amount
        print(amount, "deposited")

    # Withdraw Method
    def withdraw(self, amount):

        if amount <= self.balance:
            self.balance -= amount
            print(amount, "withdrawn")

        else:
            print("Insufficient balance")

    # Show Balance
    def show_balance(self):
        print("Balance:", self.balance)


# Object Creation
user1 = BankAccount("Vasudha", 5000)

# Initial Balance
user1.show_balance()

# Deposit
user1.deposit(2000)

# Updated Balance
user1.show_balance()

# Withdraw
user1.withdraw(3000)

# Final Balance
user1.show_balance()
```

---

# ✅ Output

```python
Balance: 5000
2000 deposited
Balance: 7000
3000 withdrawn
Balance: 4000
```

---

# 🧠 Memory Visualization

## STEP 1 — Object Creation

```python
user1 = BankAccount("Vasudha", 5000)
```

### Memory State

```text
user1
   |
   v

+-------------------+
|   BankAccount     |
+-------------------+
| name = Vasudha    |
| balance = 5000    |
+-------------------+
```

---

## STEP 2 — Deposit Operation

```python
user1.deposit(2000)
```

### Internal Calculation

```python
5000 + 2000 = 7000
```

### Updated Memory

```text
+-------------------+
| name = Vasudha    |
| balance = 7000    |
+-------------------+
```

---

## STEP 3 — Withdraw Operation

```python
user1.withdraw(3000)
```

### Internal Calculation

```python
7000 - 3000 = 4000
```

### Final Memory

```text
+-------------------+
| name = Vasudha    |
| balance = 4000    |
+-------------------+
```

---

# 📊 Final Flow Summary

| Step | Operation | Balance |
|------|------------|----------|
| 1 | Object Created | 5000 |
| 2 | Deposit 2000 | 7000 |
| 3 | Withdraw 3000 | 4000 |

---

# 🎯 Important OOP Concepts Used

| Concept | Example |
|---|---|
| Class | `BankAccount` |
| Object | `user1` |
| Constructor | `__init__()` |
| Method | `deposit()` |
| Instance Variable | `self.balance` |
| Encapsulation | Data + Methods |
| Object Reference | `user1` |

---

# 🚀 Key Takeaways

✅ Class = Blueprint

✅ Object = Real Instance

✅ `__init__()` initializes object data

✅ `self` refers to current object

✅ Methods define behavior

✅ OOP improves scalability

✅ OOP improves maintainability

---

# 🛠️ Tech Stack

- Python 3
- Object-Oriented Programming
- VS Code
- Git
- GitHub

---

# 👩‍💻 Author

## Chintada Vasudharini

Computer Science Graduate | Python Full Stack Developer | AIML | AWS 

---

# ⭐ Support

If you found this repository useful, consider giving it a ⭐ on GitHub.

---

# 📌 Future Enhancements

- Inheritance
- Polymorphism
- Encapsulation
- Abstraction
- Magic Methods
- File Handling
- Advanced OOP Projects

---

# 🔗 Connect

- GitHub: https://github.com/chintadavasudharini
- LinkedIn: https://www.linkedin.com/in/chintada-vasudharini-nov21/

---
