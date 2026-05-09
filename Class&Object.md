Python OOP Basics — Classes and Objects

A beginner-friendly collection of simple Python OOP programs demonstrating how to create classes, objects, constructors, and methods.

1. Dog Class Example
Question

Create a class called Dog

Add an __init__ method with parameters name and age, and store them as properties using self
Add a method called bark that prints the dog's name followed by " says Woof!"
Create an object d1 of the Dog class with name "Buddy" and age 3
Call the bark method on d1

Code
# Define the Dog class
class Dog:
    # Constructor
    def __init__(self, name, age):
        self.name = name
        self.age = age
    # Method
    def bark(self):
        print(self.name + " says Woof!")
# Create object
d1 = Dog("Buddy", 3)

# Call method
d1.bark()

Output
Buddy says Woof!



2. Person Class Example
Question

Create a class called Person

Add an __init__ method that takes name and age as parameters
Add a method called greet that prints "Hello, my name is " followed by the name
Create an object p1 of the class with name "John" and age 36
Call the greet method on p1

Code
# Create the Person class
class Person:
    # Constructor
    def __init__(self, name, age):
        self.name = name
        self.age = age
    # Method
    def greet(self):
        print("Hello, my name is", self.name)

# Create object
p1 = Person("John", 36)

# Call method
p1.greet()

Output
Hello, my name is John



3. Another Person Class Example
Question

Create a class called Person

Add an __init__ method that takes name and age as parameters
Add a method called greet that prints "Hello, my name is " followed by the name
Create an object p1 of the class with name "John" and age 36
Call the greet method on p1

Code
# Create a class called Person
class Person:
    # Constructor method
    def __init__(self, name, age):
        self.name = name
        self.age = age
    # Method to greet
    def greet(self):
        print("Hello, my name is", self.name)

# Create an object
p1 = Person("John", 36)

# Call the greet method
p1.greet()

Output
Hello, my name is John


Concepts Covered
Classes and Objects
Constructors (__init__)
Instance Variables
Methods in Python
Object Creation
Using self
Method Calling


Tech Stack
Language: Python 3
IDE: VS Code / PyCharm
Concepts: Object-Oriented Programming (OOP)


Author
Chintada Vasudharini
Computer Science Graduate | Python Full Stack Developer | AIML | AWS
