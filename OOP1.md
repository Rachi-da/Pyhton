Here is a set of Python exercises divided into intermediate and advanced levels. These focus on problem-solving, functions, files, exceptions, object-oriented programming, and data structures.

## Intermediate exercises

### 1. Student Grade Manager

Write a program that:

* Stores student names and grades in a dictionary.
* Allows the user to add a student.
* Displays all students and their grades.
* Calculates the class average.
* Displays the student with the highest grade.
* Displays whether each student passed or failed. A passing grade is 50 or higher.

### 2. Word Frequency Counter

Write a program that:

* Asks the user to enter a sentence.
* Removes punctuation and converts the sentence to lowercase.
* Counts how many times each word appears.
* Displays the words from most frequent to least frequent.

Example:

```text
Input: Python is easy and Python is powerful.

Output:
python: 2
is: 2
easy: 1
and: 1
powerful: 1
```

### 3. Bank Account Class

Create a class named `BankAccount` with:

* Account number
* Owner’s name
* Balance

Include methods to:

* Deposit money
* Withdraw money
* Display the account information
* Prevent withdrawals when the balance is insufficient

Raise an exception if the deposit or withdrawal amount is negative.

### 4. Employee File Processing

A file named `employees.txt` contains:

```text
101,Mary,4500
102,Ahmed,5200
103,John,3900
```

Write a program that:

* Reads the employee information from the file.
* Calculates the average salary.
* Displays employees earning above the average.
* Handles the error if the file does not exist.
* Saves the results in `salary_report.txt`.

### 5. Inventory Management System

Create a program that manages products using a dictionary. Each product has:

* Product ID
* Name
* Price
* Quantity

The program should allow the user to:

* Add a product
* Search for a product
* Update its quantity
* Sell a product
* Display products with a quantity below five
* Calculate the total value of the inventory

## Advanced exercises

### 6. Library Management System

Create the following classes:

```text
Book
Member
Library
```

The system should allow:

* Adding books and members
* Searching for books
* Borrowing and returning books
* Preventing a borrowed book from being borrowed again
* Limiting each member to three books
* Displaying overdue books
* Saving and loading the library data from a JSON file

### 7. Online Shopping System

Create classes for:

* `Product`
* `Customer`
* `ShoppingCart`
* `Order`

The program should allow customers to:

* Add and remove products from their cart
* Update product quantities
* Apply a discount code
* Calculate tax and the final price
* Check whether sufficient inventory is available
* Create and save an order receipt

Use inheritance to create at least two product types, such as:

```text
PhysicalProduct
DigitalProduct
```

### 8. Log File Analyzer

A server log contains records such as:

```text
2026-07-15 10:30:22,192.168.1.5,LOGIN_SUCCESS
2026-07-15 10:31:10,192.168.1.7,LOGIN_FAILED
2026-07-15 10:31:25,192.168.1.7,LOGIN_FAILED
```

Write a program that:

* Reads and validates the log records.
* Counts successful and failed login attempts.
* Identifies IP addresses with more than three failed attempts.
* Displays the busiest hour.
* Handles malformed records without stopping.
* Exports suspicious IP addresses to a CSV file.

### 9. Task Management Application

Create a task manager in which every task contains:

* Task ID
* Title
* Description
* Priority
* Due date
* Completion status

The program should allow the user to:

* Add, edit, delete, and complete tasks
* Search for tasks
* Sort tasks by priority or due date
* Display overdue tasks
* Save and load tasks from a JSON file

Use `datetime`, classes, exception handling, and list comprehensions.

### 10. Banking System with Inheritance

Create a base class named `Account` and two subclasses:

```text
SavingsAccount
CheckingAccount
```

Requirements:

* Every account supports deposits and withdrawals.
* A savings account earns interest.
* A checking account permits an overdraft up to a specified limit.
* Every transaction is stored in a transaction history.
* Invalid transactions raise custom exceptions.
* Account information can be saved to and loaded from a file.
* The program provides a menu for performing banking operations.

This exercise practices inheritance, polymorphism, custom exceptions, file handling, and object-oriented design.
