# Non-hashed-Password-Cracker
Non-Hashed Password Cracker is an intentionally vulnerable PHP and MySQL web application created for educational purposes to demonstrate brute-force attacks on plain-text password authentication. The project highlights authentication weaknesses caused by non-hashed password storage and lack of rate limiting.
🎯 Purpose

Demonstrate risks of non-hashed password storage

Practice brute-force attacks on login forms

Understand OWASP authentication vulnerabilities

Learn why secure password hashing is essential

⚙️ Technologies Used

PHP

MySQL

Apache (XAMPP)

HTML

✨ Features

Plain-text password storage (intentionally insecure)

Vulnerable login authentication

No rate limiting or account lockout

Suitable for brute-force testing

Simple and beginner-friendly code

📂 Project Structure
non-hashed-password-cracker/
│
├── index.html      # Login page
├── login.php       # Login validation logic
├── db.php          # Database connection
└── success.php     # Success page

🚀 How to Use (Setup & Run)
1️⃣ Download the Project
git clone https://github.com/YOUR_USERNAME/non-hashed-password-cracker.git


Or download ZIP from GitHub and extract it.

2️⃣ Install Requirements

Install XAMPP
https://www.apachefriends.org

Start Apache and MySQL from XAMPP Control Panel

3️⃣ Move Project Files

Copy the project folder to:

C:\xampp\htdocs\


Example:

C:\xampp\htdocs\non-hashed-password-cracker

4️⃣ Create Database

Open:

http://localhost/phpmyadmin


Create database:

bruteforce_lab


Select the database → SQL tab

Run:

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(50)
);

INSERT INTO users (username, password) VALUES
('admin', 'admin'),
('admin1', 'saravanan');

5️⃣ Configure Database Connection

Edit db.php if needed:

$conn = mysqli_connect("localhost", "root", "", "bruteforce_lab");

6️⃣ Run the Application

Open browser:

http://localhost/non-hashed-password-cracker/index.html

🔑 Test Credentials
Username	Password
admin	admin
admin1	saravanan

Successful login redirects to:

Successfully Hacked 🔓

🧪 Learning Outcomes

Understand brute-force login attacks

Identify authentication flaws

Practice offensive security tools (Hydra, Burp Suite)

Learn importance of password hashing and rate limiting

⚠️ Disclaimer

This project is strictly for educational purposes only.
Do NOT deploy this application in production environments.

🧠 Future Improvements

Add password hashing (bcrypt)

Implement rate limiting

Add account lockout

Input validation and prepared statements

📜 License

This project is released for educational use only.
