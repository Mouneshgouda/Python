# Python Programming - Questions and Answers

## 1. How can you connect Python to a MySQL database?
**Answer:**
To connect Python to a MySQL database, you can use the `mysql-connector` library. You need to install the library using:
```bash
pip install mysql-connector
Then, use the following code to connect to the MySQL database:

python
Copy
import mysql.connector

conn = mysql.connector.connect(
    host="your_host",
    user="your_username",
    password="your_password",
    database="your_database"
)
cursor = conn.cursor()
# Your SQL queries go here
conn.close()
2. What does the break statement do in Python loops?
Answer: The break statement is used to terminate the current loop (either for or while) immediately, regardless of whether the loop has finished iterating over all elements. After the break statement is executed, the program continues to the code after the loop.

3. What is the purpose of the return statement in a function?
Answer: The return statement is used to exit a function and return a value to the caller. Once return is executed, the function terminates, and the value specified in the return statement is sent back to the function caller.

4. What is encapsulation in OOP?
Answer: Encapsulation is a fundamental concept in Object-Oriented Programming (OOP) where the internal details of an object are hidden from the outside world. It allows you to bundle the data (attributes) and methods (functions) that operate on the data into a single unit (class), restricting direct access to some of the object's components, which can be accessed only through methods.

5. How do you import a module in Python?
Answer: You can import a module in Python using the import keyword. For example:

python
Copy
import module_name
To import a specific function or class from a module, you can use:

python
Copy
from module_name import function_name
6. Convert the list to a tuple.
Answer: Given the list:

python
Copy
nameList = ["Jhon Break", "Nelson Dia", "Miller joe"]
To convert it to a tuple, you can use:

python
Copy
nameTuple = tuple(nameList)
print(nameTuple)
Output:

arduino
Copy
('Jhon Break', 'Nelson Dia', 'Miller joe')
7. Consider the following Python code:
python
Copy
def myFun(x, y=50):
    print("x:", x)
    print("y:", y)

myFun(10)
8. What output do you expect from the above code?
Answer: The function myFun takes two parameters, with y having a default value of 50. Since the argument 10 is provided for x, and y is not provided, it will use the default value for y. The output will be:

makefile
Copy
x: 10
y: 50
9. State any 2 popular applications of Python.
Answer:

Web Development: Frameworks like Django and Flask are used to develop robust web applications.
Data Science: Libraries like Pandas, NumPy, and Matplotlib are used for data analysis and visualization.
10. How do you define a function in Python?
Which of the following is correct?

A. function my_function()
B. def my_function():
C. function: my_function()
D. def: my_function()
Answer: The correct way to define a function in Python is option B:

python
Copy
def my_function():
    pass
11. What is polymorphism in Object-Oriented Programming?
Answer: Polymorphism in OOP refers to the ability of different objects to respond to the same method call in a way that is appropriate to their type. It allows a single function or method to work with objects of different types, making the code more flexible and extensible.

12. Define a Python module.
Answer: A Python module is a file that contains Python code (functions, classes, variables, and runnable code) which can be imported and used in other Python programs. Modules allow for better organization and reusability of code.
