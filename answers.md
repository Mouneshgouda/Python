 ## 1.How can you connect Python to a MySQL database?

 You can connect Python to a MySQL database using the mysql-connector-python library. First, install the library with pip install mysql-connector-python and then use the mysql.connector.connect() method to establish a connection to the 
 database.

## 2. What does the break statement do in Python loops?
 The break statement is used to exit or terminate the current loop (for or while) prematurely, even if the loop's condition hasn't been satisfied yet.

## 3.What is the purpose of the return statement in a function?
 The return statement is used to exit a function and optionally pass a value back to the caller.

## 4. What is encapsulation in OOP?
 Encapsulation is the concept of bundling the data (variables) and methods (functions) that operate on the data into a single unit, or class. It restricts direct access to some of the object's components and can prevent the accidental 
 modification of data by outside code.

## 5How do you import a module in Python?
- You can import a module in Python using the import keyword, like this:

python
```
import module_name
```
### 1. How can you connect Python to a MySQL database?
To connect Python to a MySQL database, you can use the `mysql-connector` library. You can install it using pip:
```
pip install mysql-connector
Once installed, use the following code to connect:


import mysql.connector

conn = mysql.connector.connect(
    host="localhost",
    user="root",
    password="your_password",
    database="your_database"
)
```
### 2. What does the break statement do in Python loops?
The break statement is used to terminate the current loop (for or while) immediately, skipping any remaining iterations. After the break is executed, the program continues with the next statement after the loop.
```
Example:

for i in range(10):
    if i == 5:
        break  # Stops the loop when i is 5
    print(i)
```
### 3. What is the purpose of the return statement in a function?
The return statement is used to exit a function and return a value from that function to the calling code. If no value is specified, the function returns None by default.
```
Example:

python
Copy
def add(a, b):
    return a + b

result = add(5, 3)
print(result)  # Output: 8
```
### 4. What is encapsulation in OOP?
 Encapsulation is an object-oriented programming (OOP) concept where the data (attributes) and the methods (functions) that manipulate the data are bundled together in a class. It helps 
 protect the internal state of an object by restricting access to certain components.

### 5. How do you import a module in Python?
You can import a module using the import keyword:
import module_name
To import a specific function or class from a module:

```
from module_name import function_name
Example:

python
Copy
import math
print(math.sqrt(16))  # Output: 4.0
```
### 6. Convert the following list to a tuple:
```
nameList = ["Jhon Break", "Nelson Dia", "Miller joe"]
nameTuple = tuple(nameList)
print(nameTuple)
```
### 7. Consider the following Python code:
```
def myFun(x, y=50):
    print("x:", x)
    print("y:", y)

myFun(10)
```
### 8. What output do you expect from the above code?
The output of the above code will be:

x: 10
y: 50
Since the function myFun is called with a value for x, but no value for y, it uses the default value of y which is 50.

9. State any 2 popular applications of Python.
Web Development: Python is widely used for web development, with frameworks like Django and Flask.
Data Science and Machine Learning: Python is one of the most popular languages for data analysis and machine learning, with libraries such as Pandas, NumPy, and TensorFlow.
10. How do you define a function in Python?
The correct way to define a function in Python is:
B. def my_function():


def my_function():
    print("Hello, World!")
11. What is polymorphism in Object-Oriented Programming?
Polymorphism is an OOP concept where objects of different classes can be treated as objects of a common superclass. It allows methods to be used in multiple forms. This can be achieved through method overriding or method overloading.

Example:

python
Copy
class Dog:
    def speak(self):
        return "Woof"

class Cat:
    def speak(self):
        return "Meow"

def animal_sound(animal):
    print(animal.speak())

dog = Dog()
cat = Cat()

animal_sound(dog)  # Output: Woof
animal_sound(cat)  # Output: Meow
12. Define a Python module.
A Python module is a file containing Python definitions and statements. It can define functions, classes, and variables that can be used in other Python scripts. Python modules help organize and reuse code.

Example of creating a module (my_module.py):

python
Copy
# my_module.py
def greet():
    print("Hello from the module!")
To use it in another script:

python
Copy
import my_module
my_module.greet()
