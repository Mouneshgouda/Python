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
- `deposit(amount)`: Deposits the given amount into the account. Returns a success message with the updated balance.
- `withdraw(amount)`: Withdraws the given amount from the account if the balance is sufficient. Returns a success message with the updated balance, or a message indicating insufficient balance.
- `details()`: Returns a string displaying the account number, customer details, and current balance.

### 3. Bank Class

The `Bank` class manages multiple bank accounts and provides methods to add accounts, retrieve accounts, and get the number of accounts in the bank.

#### Attributes:
- `accounts` (dictionary): A dictionary to store all bank accounts, with the `account_number` as the key and `BankAccount` objects as values.

#### Constructor (`__init__`):
- Initializes an empty dictionary `accounts` to store the bank accounts.

#### Methods:
- `add_account(account)`: Adds a new account to the bank. Returns a message confirming that the account has been added.
- `get_account(account_number)`: Retrieves the account details for a given `account_number`. If the account exists, returns its details; otherwise, returns an "Account not found" message.
- `info()`: Returns the total number of accounts currently in the bank.
