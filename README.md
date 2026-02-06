
🏦Banking System (C++ Console Application)
📌 Overview

The ABA Banking System is a console-based C++ application that simulates basic banking operations.
Users can create accounts, log in securely, and perform banking actions such as checking balance, depositing money, withdrawing funds, and changing their PIN.

This project demonstrates:

Structured programming

User authentication

Menu-driven systems

Use of struct, functions, loops, and conditionals in C++

✨ Features
🔐 Account Creation

Minimum age requirement: 15 years old

Initial balance rules:

Age 15–19 → $100

Age 20+ → $1000

Each user has:

Name

ID

Age

PIN

Balance

🔑 Login System

Secure login using:

Name

ID

Age

PIN

Maximum 3 login attempts

Automatically returns to the main menu after failed attempts

💳 Banking Menu (After Login)

Once logged in, users can:

Check Balance

Deposit Money

Withdraw Money

Prevents overdraft

Change PIN

Requires current PIN

Option to cancel

Exit to Main Menu

🚪 Exit System

Clean exit from both:

User banking menu

Main program
🧠 Program Structure
📦 Data Structure
struct User {
    string name;
    string id;
    int age, pin;
    double balance;
};
🔧 Core Functions
Function
| Function          | Description                 |
| ----------------- | --------------------------- |
| `startMenu()`     | Displays the main menu      |
| `createUser()`    | Applies age & balance rules |
| `createAccount()` | Collects user data          |
| `login()`         | Authenticates users         |
| `user()`          | Displays banking menu       |
| `balance()`       | Shows user balance          |
| `deposite()`      | Adds money to balance       |
| `withdrawal()`    | Withdraws money safely      |
| `changePIN()`     | Updates PIN securely        |
🔁 Program Flow

User sees Start Menu

Choose:

Create Account

Login

Exit

After login:

Access banking features

Exit safely back to main menu or program

🛠 Technologies Used

Language: C++

Libraries:

<iostream>

<string>

<iomanip>

<cstdlib>

✅ Key Concepts Demonstrated

Functions with references

Arrays of structs

Input validation

Loop control (do-while)

Menu-driven logic

Authentication flow

Clean exit conditions

🚀 Future Improvements

File storage (save users permanently)

Password masking for PIN

Admin account

Transaction history

Better input validation (non-numeric input)
