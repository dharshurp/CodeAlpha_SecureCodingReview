📄 Secure Coding Review – Task 3

🔐 Project Title

Secure Code Review of Password Manager Application

📌 Overview
This project focuses on analyzing a Python-based password manager application to identify security vulnerabilities and improve secure coding practices. The review includes manual inspection and basic security analysis to understand common risks in software development.

🎯 Objective
Identify security flaws in the application
Understand insecure coding practices
Apply secure coding recommendations
Improve awareness of cybersecurity risks

🛠 Tools Used
Python 3
Cryptography (Fernet encryption)
Pydroid 3 / VS Code
Manual Code Review

💻 Project Description
The application is a simple password manager that:
Allows user login using a master password
Stores passwords in encrypted format
Saves data in a local JSON file
Retrieves and decrypts stored passwords

⚙️ Features
Secure login system
Password encryption using Fernet
Add and view stored passwords
Local data storage

🚨 Security Issues Identified

🔴 1. Hardcoded Password Risk
Default password is visible in code which is insecure.

🔴 2. Weak Authentication
Only single password-based login is used.

🟠 3. Key Storage Issue
Encryption key stored locally in a file.

🟠 4. No Password Hashing
Passwords are not hashed before usage.

🟡 5. Limited Input Validation
User inputs are not fully validated.

🔧 Recommendations

Use environment variables for sensitive data
Implement bcrypt password hashing
Store encryption keys securely (vault/system keychain)
Add account lockout after failed attempts
Improve input validation

📊 Outcome
This project helped in understanding real-world security vulnerabilities in applications and improved knowledge of secure coding practices.

👨‍💻 Author
Dharshini R P
Cyber Security Intern
CodeAlpha Internship Program
