
# Python OOP Essentials 🚀

## Overview

Python is an object-oriented programming language that helps developers build scalable, reusable, and maintainable applications.
Using **Classes** and **Objects**, we can model real-world systems efficiently while improving code organization and readability.

### Key Advantages of OOP

* Code Reusability
* Better Maintainability
* Improved Scalability
* Data Security through Encapsulation
* Real-world Modeling
* Modular Development

---

# 1. Class

A **Class** is a blueprint used to create objects.
It defines:

* **Attributes** → Variables inside a class
* **Methods** → Functions inside a class

## Example

```python
class Student:
    name = "Vasudha"
    age = 23

print(Student.name)
print(Student.age)
```

### Output

```python
Vasudha
23
```

---

# 2. Object

An **Object** is an instance of a class.
Objects inherit all attributes and methods defined inside the class.

## Example

```python
class Student:
    name = "Vasudha"
    age = 23

s1 = Student()

print(s1.name)
print(s1.age)
```

### Output

```python
Vasudha
23
```

---

# 3. The `pass` Statement

Python classes cannot be empty.
Use the `pass` keyword when creating a placeholder class.

## Example

```python
class Person:
    pass
```

---

# 4. Constructor - `__init__()`

The `__init__()` method is a special constructor method automatically executed when an object is created.

### Purpose

* Initialize object attributes
* Assign values during object creation
* Execute startup logic

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

### Output

```python
Vasu
23
```

---

# 5. Default Parameters in `__init__()`

Constructors can contain default values.

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

### Output

```python
Vasu 18
Vasudharini 23
```

---

# 6. Multiple Parameters in Constructor

The constructor can accept multiple parameters.

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
print(p1.city)
```

---

# 7. Methods in Classes

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

### Output

```python
Name: Vasudha
Age: 23
```

---

# 8. Real-world Example - Dog Class

```python
class Dog:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(self.name + " says Woof!")


d1 = Dog("Buddy", 3)
d1.bark()
```

### Output

```python
Buddy says Woof!
```

---

# 9. Why `self` is Important

`self` refers to the current object instance.
It is used to:

* Access object variables
* Access methods
* Differentiate instance variables from local variables

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

### Output

```python
Hello, my name is Vasu
```

---

# 10. `self` Can Have Any Name

The first parameter can technically have any name, though `self` is the Python convention.

## Example

```python
class Person:

    def __init__(myobject, name, age):
        myobject.name = name
        myobject.age = age

    def greet(abc):
        print("Hello, my name is", abc.name)

p1 = Person("Vasu", 23)
p1.greet()
```

---

# 11. Calling Methods Inside Methods

Methods can call other methods using `self`.

## Example

```python
class Person:

    def __init__(self, name):
        self.name = name

    def greet(self):
        return "Hello, " + self.name

    def welcome(self):
        message = self.greet()
        print(message + "! Welcome to our website.")

p1 = Person("Vasu")
p1.welcome()
```

### Output

```python
Hello, Vasu! Welcome to our website.
```

---

# 12. Real-world Project Example - Bank Account

```python
class BankAccount:

    def __init__(self, name, balance):
        self.name = name
        self.balance = balance

    def deposit(self, amount):
        self.balance += amount
        print(amount, "deposited")

    def withdraw(self, amount):
        if amount <= self.balance:
            self.balance -= amount
            print(amount, "withdrawn")
        else:
            print("Insufficient balance")

    def show_balance(self):
        print("Balance:", self.balance)


user1 = BankAccount("Vasudha", 5000)

user1.deposit(2000)
user1.show_balance()
user1.withdraw(3000)
user1.show_balance()
```

---

# 13. Class Variables vs Instance Variables

## Class Variables

* Shared among all objects
* Defined directly inside the class

## Instance Variables

* Unique for each object
* Defined inside `__init__()` using `self`

## Example

```python
class Person:

    lastname = ""

    def __init__(self, name):
        self.name = name

    def show_name(self):
        print(f"Hello, I'm {self.name} {self.lastname}")


p1 = Person("Vasu")
p2 = Person("Vasudha")

Person.lastname = "Ch"

print(p1.lastname)
print(p2.lastname)

p1.show_name()
```

### Output

```python
Ch
Ch
Hello, I'm Vasu Ch
```

---

# Key Takeaways

✅ Classes are blueprints

✅ Objects are real instances of classes

✅ `__init__()` initializes object data

✅ `self` refers to the current object

✅ Methods define object behavior

✅ OOP improves scalability and code reusability

---

# Tech Stack

* Python 
* Object-Oriented Programming (OOP)


---

# Author

### Chintada Vasudharini

Computer Science Graduate | Python Full Stack Developer | AIML | AWS

---

⭐ If you found this repository useful, give it a star on GitHub.
