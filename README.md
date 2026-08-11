# Tourist Management System – A Travel Platform

📌 Overview
Tourist Management System is a web application built using PHP and MySQL to manage tour package bookings, user accounts, and payment records.

It allows users to register, browse travel packages, and book tours online, while providing administrators with a dashboard to manage package offerings, user profiles, and payment histories.

✨ Features

👤 User Features
* User registration, login, and secure logout
* Browse available travel packages with details and prices
* Book and purchase tour packages
* View booking and account information

🛡️ Admin Features
* Centralized administrator dashboard
* Manage Packages: Add, edit, or delete tour packages
* Manage Users: View and update registered user accounts
* Payment History: Track user purchases and payment logs

🏗️ Project Structure

Tourist-Management-System-main/
│
├── admin/                     # Admin dashboard & management scripts
│   ├── dashboard.php
│   ├── manage_packages.php
│   ├── manage_packages_section.php
│   ├── manage_users.php
│   ├── manage_users_section.php
│   ├── payment_history_section.php
│   └── update_user.php
│
├── images/                    # Project image assets
│
├── includes/                  # Database connection & shared components
│   ├── db.php
│   ├── footer.php
│   ├── functions.php
│   └── navbar.php
│
├── sql/                       # Database schema
│   └── database.sql
│
├── index.php                  # Homepage
├── login.php                  # User login page
├── logout.php                 # User logout handler
├── packages.php               # Travel packages list
├── purchase.php               # Package booking handler
├── register.php               # User registration page
└── s.css                      # Custom stylesheet

🛠️ Technologies Used

* **Language:** PHP, HTML5, CSS3, JavaScript
* **Database:** MySQL / MariaDB
* **Server Environment:** Apache (XAMPP / WAMP)
* **Version Control:** Git & GitHub

🔄 Application Workflow

                  ┌───────────────────┐
                  │      Register     │
                  └─────────┬─────────┘
                            │
                            ▼
                  ┌───────────────────┐
                  │       Login       │
                  └─────────┬─────────┘
                            │
                            ▼
                  ┌───────────────────┐
                  │     Home Page     │
                  └─────────┬─────────┘
                            │
               ┌────────────┴────────────┐
               │                         │
               ▼                         ▼
       ┌───────────────┐        ┌────────────────┐
       │Browse Packages│        │ Admin Panel    │
       └───────┬───────┘        └───────┬────────┘
               │                        │
               ▼                        ▼
       ┌───────────────┐        ┌────────────────┐
       │Purchase Package│       │Manage Packages │
       └───────┬───────┘        │ & Payments     │
               │                        └────────────────┘
               ▼
       ┌───────────────┐
       │Payment Record │
       └───────────────┘

🚀 Getting Started

Prerequisites
* XAMPP (or any local Apache + MySQL web server)
* PHP 7.4+ or 8.+
* Web browser

1. Clone the Repository
git clone https://github.com/Iftekharul756/Tourist_Management_System_DBMS.git

2. Move to Local Server Directory
Copy the project folder into your web server's root directory:
C:\xampp\htdocs\Tourist-Management-System-main\

3. Start Apache & MySQL
Launch XAMPP Control Panel and click "Start" for Apache and MySQL.

4. Setup Database
1. Open phpMyAdmin in your browser: http://localhost/phpmyadmin/
2. Create a database named `tourist_management`.
3. Click Import, choose `sql/database.sql` from the project folder, and click Go.

5. Verify Database Connection
Check `includes/db.php` to ensure settings match your MySQL configuration:
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "tourist_management";

6. Run the Application
Open your web browser and visit:
http://localhost/Tourist-Management-System-main/index.php

🔐 User Roles

Customer / User
* Register and log in
* Browse tour packages
* Purchase packages
* View booking records

Administrator
* Access the admin panel (`/admin/dashboard.php`)
* Add, edit, and delete packages
* Manage user accounts
* View payment histories

📚 Key Concepts Demonstrated

* Full-stack PHP & MySQL development
* Relational Database Management Systems (DBMS)
* Session-based user authentication & authorization
* CRUD (Create, Read, Update, Delete) operations
* Form validation & database script integration
* Git & GitHub version control

👨‍💻 Author

Md Iftekharul Alam
B.Sc. in Computer Science & Engineering
Interested in Artificial Intelligence, Machine Learning, Data, and Software Development.

⭐ Support

If you find this project helpful, consider giving the repository a ⭐!
