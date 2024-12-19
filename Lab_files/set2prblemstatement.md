#Class Descriptions
- 1. Customer Class
  Attributes:

- name (string): The name of the customer.
  address (string): The address of the customer.
  contact (string): The contact number of the customer.
  Constructor (__init__):

- The constructor initializes the name, address, and contact attributes.
  Method:

- details(): Returns a string displaying the customer's name, address, and contact.
- 2. BankAccount Class
  Attributes:

- account_number (string): The unique identifier for the account.
  customer (Customer object): The customer associated with this bank account.
  balance (float, default=0): The initial balance in the account (default is 0).
  Constructor (__init__):

  The constructor initializes the account_number, customer, and balance attributes.
  Methods:

- deposit(amount): Deposits the given amount into the account. Returns a success message with the updated balance.
- withdraw(amount): Withdraws the given amount from the account if the balance is sufficient. Returns a success message with the updated balance, or a message indicating insufficient 
  balance.
- details(): Returns a string displaying the account number, customer details, and current balance.
- 3. Bank Class
  Attributes:

- accounts (dictionary): A dictionary to store all bank accounts, with the account_number as the key and BankAccount objects as values.
  Constructor (__init__):

- The constructor initializes an empty dictionary accounts to store the bank accounts.
  Methods:

- add_account(account): Adds a new account to the bank. Returns a message confirming that the account has been added.
  get_account(account_number): Retrieves the account details for a given account_number. If the account exists, return its details; otherwise, return an "Account not found" message.
  info(): Returns the total number of accounts currently in the bank.
