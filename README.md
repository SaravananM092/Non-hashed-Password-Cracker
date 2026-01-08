# 🔐 **NON-HASHED PASSWORD CRACKER**

## 📌 **OVERVIEW**
**Non-Hashed Password Cracker** is an intentionally vulnerable web application created for **educational and training purposes**. This project demonstrates how storing passwords in **plain text (non-hashed)** and lacking basic security controls can lead to **brute-force and authentication attacks**.

---

## 🎯 **PROJECT PURPOSE**
- **Demonstrate risks of non-hashed password storage**
- **Practice brute-force attacks on login forms**
- **Understand OWASP authentication vulnerabilities**
- **Learn why secure password hashing is essential**

---

## ⚙️ **TECHNOLOGIES USED**
- **PHP**
- **MySQL**
- **Apache (XAMPP)**
- **HTML**

---

## ✨ **FEATURES**
- **Plain-text password storage (intentionally insecure)**
- **Vulnerable login authentication**
- **No rate limiting or account lockout**
- **Brute-force friendly environment**
- **Beginner-friendly source code**

---

## 📂 **PROJECT STRUCTURE**
non-hashed-password-cracker/
│
├── index.html # Login Page 

├── login.php # Authentication Logic

├── db.php # Database Connection

└── success.php # Success Page

yaml
Copy code

---

## 🚀 **HOW TO USE (SETUP & RUN)**

### **1️⃣ DOWNLOAD THE PROJECT**
```bash

git clone https://github.com/YOUR_USERNAME/non-hashed-password-cracker.git

OR download ZIP from GitHub and extract it.

### **2️⃣ INSTALL REQUIREMENTS**
Install XAMPP

https://www.apachefriends.org

Start Apache and MySQL from XAMPP Control Panel

### **3️⃣ MOVE PROJECT FILES**
Copy the project folder to:

makefile
Copy code
C:\xampp\htdocs\
Example:

makefile
Copy code
C:\xampp\htdocs\non-hashed-password-cracker
4️⃣ CREATE DATABASE
Open:

arduino
Copy code
http://localhost/phpmyadmin
Create database:

nginx
Copy code
bruteforce_lab
Select the database → SQL TAB

Paste and run:

sql
Copy code
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(50)
);

INSERT INTO users (username, password) VALUES
('admin', 'admin'),
('admin1', 'saravanan');
5️⃣ CONFIGURE DATABASE CONNECTION
Open db.php and verify:

php
Copy code
$conn = mysqli_connect("localhost", "root", "", "bruteforce_lab");
6️⃣ RUN THE APPLICATION
Open browser:

pgsql
Copy code
http://localhost/non-hashed-password-cracker/index.html
🔑 TEST CREDENTIALS
USERNAME	PASSWORD
admin	admin
admin1	saravanan

Successful login redirects to:
👉 Successfully Hacked 🔓

🧪 LEARNING OUTCOMES
Understand brute-force login attacks

Identify authentication flaws

Practice penetration testing tools

Learn importance of password hashing

⚠️ DISCLAIMER
This project is strictly for educational purposes only.
Do NOT deploy this application in production environments.

🧠 FUTURE IMPROVEMENTS
Implement password hashing (bcrypt)

Add rate limiting

Account lockout mechanisms

Prepared statements & input validation

📜 LICENSE
This project is released for educational and training use only.

yaml
Copy code

---

### ✅ **What to Do Now**
1. Open your GitHub repo  
2. Click **README.md → Edit**
3. **Paste everything above**
4. Click **Commit changes**

---
