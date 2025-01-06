# 1 Bank Account Management System

## Class Descriptions

### 1. Customer Class

The `Customer` class represents a customer of the bank with their basic details.

#### Attributes:
- `name` (string): The name of the customer.
- `address` (string): The address of the customer.
- `contact` (string): The contact number of the customer.

#### Constructor (`__init__`):
- Initializes the `name`, `address`, and `contact` attributes.

#### Method:
- `details()`: Returns a string displaying the customer's name, address, and contact.

### 2. BankAccount Class

The `BankAccount` class represents a bank account and allows basic operations like deposits and withdrawals.

#### Attributes:
- `account_number` (string): The unique identifier for the account.
- `customer` (Customer object): The customer associated with the bank account.
- `balance` (float, default=0): The initial balance in the account (default is 0).

#### Constructor (`__init__`):
- Initializes the `account_number`, `customer`, and `balance` attributes.

#### Methods:
- `deposit(amount)`: Deposits the given amount into the account. Returns a success message with the updated balance.self,amount,balance,+=
- return amount ,self.balance
- `withdraw(amount)`: Withdraws the given amount from the account if the balance is sufficient. Returns a success message with the updated balance, or a message indicating insufficient balance.amount,<,=,self.balance,self.balance,-=,amount
- return
- `details()`: Returns a string displaying the account number, customer.details, and current s.balance.

### 3. Bank Class

The `Bank` class manages multiple bank accounts and provides methods to add accounts, retrieve accounts, and get the number of accounts in the bank.

#### Attributes:
- `accounts` (dictionary): A dictionary to store all bank accounts, with the `account_number` as the key and `BankAccount` objects as values.
#### Constructor (`__init__`):
- Initializes an empty dictionary `accounts` to store the bank accounts.self.accounts={}

#### Methods:
- `add_account(account)`: Adds a new account to the bank. Returns a message confirming that the account has been added.self,acounts,[],account.accountnumber,=acount
- return account.account_number
- `get_account(account_number)`: Retrieves the account details for a given `account_number`. If the account exists, returns its details; otherwise, returns an "Account not found" message.
- return self.accounts.get(account_number, "Account not found.")
- `info()`: Returns the total number of accounts currently in the bank.
- return f"Number of Accounts: {len(self.accounts)}"


# School Management System

## Objective:
You are tasked with creating a system to manage students, teachers, and courses at a school. The system will consist of three main components: **Student**, **Teacher**, and **Course** classes. These classes will be used to represent and manage the information about students, teachers, and the courses they are enrolled in.

## Classes and Attributes

### 1. Student Class
Represents a student enrolled in the school.

#### Attributes:
- `name` (string): The name of the student.
- `grade` (string): The grade or class the student is in.

#### Constructor (`__init__`):
- Initializes the `name` and `grade` attributes.

#### Method:
- `get_details()`: Returns a string that provides the student's name and grade.

### 2. Teacher Class
Represents a teacher employed at the school.

#### Attributes:
- `name` (string): The name of the teacher.
- `subject` (string): The subject taught by the teacher.

#### Constructor (`__init__`):
- Initializes the `name` and `subject` attributes.

#### Method:
- `get_details()`: Returns a string that provides the teacher's name and subject.

### 3. Course Class
Represents a course that is being taught at the school.

#### Attributes:
- `name` (string): The name of the course (e.g., Math, Science).
- `teacher` (Teacher object): The teacher who is teaching this course.
- `students` (list): A list of `Student` objects enrolled in the course.

#### Constructor (`__init__`):
- Initializes the `name` of the course, `teacher` (Teacher object), and an empty list `students` to store enrolled students.

#### Methods:
- `enroll_student(student)`: Adds a `Student` object to the `students` list, enrolling the student in the course.          self.students.append(student)

- `list_students()`: Returns a list of student names who are enrolled in the course.
-         return [student.name for student in self.students]

-  # Example usage:
student1 = Student("Sad", 10)
student2 = Student("Ego", 11)

teacher1 = Teacher("The Creator:-God ", "Love and Peace")

course1 = Course("Love and Peace", teacher1)
course1.enroll_student(student1)
course1.enroll_student(student2)

# Print student details
for student in [student1, student2]:
    print(student.get_details())
    print(f"Enrolled in {course1.name} taught by {teacher1.name}\n")   




