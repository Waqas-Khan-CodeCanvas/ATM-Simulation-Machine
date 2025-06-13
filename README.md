[//]: # "# ATM Simulation System"
[//]: #
[//]: # "## Overview"
[//]: # "The ATM Simulation System is a Java-based console application that simulates the functionality of a real-world Automated Teller Machine (ATM). This project demonstrates object-oriented programming principles while providing a functional banking simulation."
[//]: #
[//]: # "## Features"
[//]: # "- User account creation and management"
[//]: # "- Secure authentication system"
[//]: # "- Core banking operations (deposit, withdrawal)"
[//]: # "- Transaction history tracking"
[//]: # "- Profile management"
[//]: # "- Password reset functionality"
[//]: # "- File-based data persistence"
[//]: #
[//]: # "## Technologies Used"
[//]: #
[//]: # "### Java Core Features"
[//]: # "- Java SE (Standard Edition)"
[//]: # "- Console-based user interface using java.util.Scanner"
[//]: # "- File I/O operations for data persistence"
[//]: #
[//]: # "### Object-Oriented Programming Concepts"
[//]: # "- **Encapsulation**: Private fields with public getters/setters in all model classes"
[//]: # "- **Polymorphism**: Interface-based polymorphism through IAccountOperations and IDatabaseOperations"
[//]: # "- **Abstraction**: Interfaces defining operations implemented by concrete classes"
[//]: # "- **Interface Implementation**: IAccountOperations and IDatabaseOperations"
[//]: # "- **Data Modeling**: Model classes (User, Account, Transaction) and Enum (TransactionType)"
[//]: #
[//]: # "## Project Architecture"
[//]: #
[//]: # "The project follows a layered architecture:"
[//]: #
[//]: # "1. **Presentation Layer**: ATM class handles user interaction"
[//]: # "2. **Business Logic Layer**: AccountManager implements account operations"
[//]: # "3. **Data Access Layer**: DatabaseManager handles data persistence"
[//]: # "4. **Model Layer**: User, Account, and Transaction classes represent data entities"
[//]: #
[//]: # "### Design Patterns"
[//]: # "- Interface-based Programming"
[//]: # "- Singleton Pattern (implicit in the ATM class)"
[//]: # "- Repository Pattern (DatabaseManager)"
[//]: #
[//]: # "## Project Structure"

# 💳 ATM Simulation System

A console-based Java application that simulates core ATM functionalities such as user account creation, login, secure transactions, and data persistence.

---

## 🎯 Project Objectives

- ✅ Simulate real-world ATM banking operations
- 🔒 Implement secure user authentication
- 📁 Maintain transaction history with timestamps and IDs
- 💬 Provide a user-friendly console interface
- 💡 Demonstrate Java OOP principles
- 🧾 Use file-based storage for persistent data

---

## 🛠️ Technologies Used

- **Java SE (Standard Edition)**
- **Console Input**: `java.util.Scanner`
- **File I/O**: Java file handling for data persistence

### Java OOP Concepts

- **Encapsulation**: Private fields with public getters/setters (`User`, `Account`, `Transaction`)
- **Abstraction**: Interfaces like `IAccountOperations`, `IDatabaseOperations`
- **Polymorphism**: Interface-based polymorphism
- **Inheritance**: Extensible class architecture

### Design Patterns

- **Interface-Based Programming**
- **Singleton Pattern** (ATM class)
- **Repository Pattern** (DatabaseManager)

---

## 🧱 System Architecture

```
Presentation Layer      -> ATM (User Interaction)
Business Logic Layer    -> AccountManager (Banking Operations)
Data Access Layer       -> DatabaseManager (File I/O)
Model Layer             -> User, Account, Transaction, TransactionType
```

---

## 🚀 Development Process

1. **Requirements Analysis** - Define ATM functionalities
2. **Class Design** - Design model classes and interfaces
3. **Implementation** - Develop core features
4. **Testing** - Manual scenario-based testing
5. **Refinement** - Optimize and debug

---

## 🧩 Challenges & Solutions

| 🔧 Challenge           | ✅ Solution                                                         |
| ---------------------- | ------------------------------------------------------------------- |
| Data Persistence       | Implemented text file storage in `src/Accounts_db`                  |
| Transaction Management | Created a `Transaction` class with unique ID and timestamp          |
| User Authentication    | Built simple and secure username/password authentication system     |
| Memory Efficiency      | Cached user data in memory to reduce file I/O via `DatabaseManager` |

---

## 📖 User Guide

### ▶️ Running the Application

1. **Compile the files:**

   ```bash
   javac *.java
   ```

2. **Run the application:**

   ```bash
   java ATM
   ```

3. **(Optional) Create and run JAR:**
   ```bash
   jar cvfe ATM.jar ATM *.class
   java -jar ATM.jar
   ```

---

### 🧭 Main Menu

Upon running the app, you'll see:

1. Login Account
2. Create Account
3. Exit

---

### 🆕 Create a New Account

You will be prompted to enter:

- Full Name
- Username
- Age
- Contact Number
- ID Card Number
- Password
- City
- Email
- Home Address
- Account Purpose
- Initial Deposit Amount

---

### 🔐 Login to Existing Account

- Enter your **username** and **password** to proceed

---

### 🏦 Available Operations After Login

1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Show Profile
5. Reset Password
6. Transaction History
7. Logout

---

## 🗂️ Project Deployment

### ⚙️ Running as a Standalone App

- Requires: **JRE 8 or higher**
- Supported OS: **Any OS with Java support**
- Storage: **~50MB disk space**
- Memory: **512MB RAM recommended**

### 📂 Data Storage Structure

- Path: `src/Accounts_db/`
- Each user has a folder named after their **username**
- All user data and transaction logs are stored in plain text files
- Directory structure is created automatically if not present

---

## 🙏 Acknowledgements

This project was built to demonstrate core Java concepts and simulate the real-world operations of an ATM system in a secure, efficient, and educational manner.

---

> 💬 **Have fun exploring the ATM Simulation System!**
