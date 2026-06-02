# 🔐 Secure Coding Review - Password Manager

## 📌 Overview 
This project analyzes a Python-based password manager application to identify security vulnerabilities and improve secure coding practices.

The goal is to understand real-world security risks and apply secure coding principles.

---

## 🧩 Project Description
The application is a simple password manager that:
- Allows login using a master password  
- Stores passwords using encryption (Fernet)  
- Saves data in a local JSON file  
- Retrieves and decrypts stored passwords  

---

## ⚠️ Security Issues Identified

### 1. Hardcoded Password Risk
Default password is visible in code, making it insecure.

### 2. Weak Authentication
Only a single master password is used for authentication.

### 3. Encryption Key Storage Issue
Encryption key is stored locally in a file, which can be accessed.

### 4. No Password Hashing
Passwords are not hashed before storage or validation.

### 5. Limited Input Validation
User inputs are not properly validated, increasing risk of misuse.

---

## 🛠️ Recommendations

- Use environment variables for sensitive data  
- Implement bcrypt for password hashing  
- Store encryption keys securely (OS keychain / vault)  
- Add account lockout after multiple failed attempts  
- Improve input validation and sanitization  

---

## 📊 Outcome
This project helped in understanding real-world application vulnerabilities and improved knowledge of secure coding practices such as authentication security, encryption handling, and input validation.

---

## 👩‍💻 Author
Dharshini R P  
Cyber Security Intern - CodeAlpha
