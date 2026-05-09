# Python OOP Basics — Classes and Objects


A clean and beginner-friendly collection of Python Object-Oriented Programming (OOP) examples demonstrating:

- Classes and Objects
- Constructors (`__init__`)
- Instance Variables
- Methods
- Object Creation
- Method Calling

---

# 📌 Table of Contents

1. [Dog Class Example](#-1-dog-class-example)
2. [Person Class Example](#-2-person-class-example)
3. [Another Person Class Example](#-3-another-person-class-example)
4. [Concepts Covered](#-concepts-covered)
5. [Tech Stack](#-tech-stack)
6. [Author](#-author)

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

## 💻 Code

```python
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
```

---

## ✅ Output

```python
Buddy says Woof!
```

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

## 💻 Code

```python
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
```

---

## ✅ Output

```python
Hello, my name is John
```

---

# 👨‍💻 3. Another Person Class Example

## 📝 Question

Create a class called `Person`

- Add an `__init__` method that takes `name` and `age`
- Add a method called `greet`
- Print `"Hello, my name is"` followed by the name
- Create an object `p1`
- Call the `greet()` method

---

## 💻 Code

```python
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
```

---

## ✅ Output

```python
Hello, my name is John
```

---

# 📚 Concepts Covered

| Concept | Description |
|----------|-------------|
| Class | Blueprint for creating objects |
| Object | Instance of a class |
| Constructor | Special method used to initialize objects |
| `self` Keyword | Refers to the current object |
| Instance Variables | Variables unique to each object |
| Methods | Functions defined inside a class |
| Object Creation | Creating class instances |
| Method Calling | Executing class methods |

---

# 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| Python 3 | Programming Language |
| VS Code | Development Environment |
| PyCharm | IDE |
| Git & GitHub | Version Control |

---

## Getting Started

Clone the repository:

```bash
git clone https://github.com/chintadavasudharini/python.git
```

Navigate to the project folder:

```bash
cd python
```

Run any Python file:

```bash
python filename.py
```

---



# 📖 Learning Outcomes

After completing these examples, you will understand:

- How classes work in Python
- How to create objects
- How constructors initialize data
- How methods operate inside classes
- Basic principles of Object-Oriented Programming

---



---

# 👩‍💻 Author

## Chintada Vasudharini

Computer Science Graduate  
Python Full Stack Developer | AIML | AWS
GitHub: https://github.com/chintadavasudharini
---

# ⭐ Support

If you found this project useful:

- ⭐ Star the repository
- 🍴 Fork the project
- 📢 Share with others
- 💡 Contribute improvements

---
