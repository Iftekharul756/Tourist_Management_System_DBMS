# Tourist_Management_System - A Web-Based Travel & DBMS Platform

📌 Overview
Tourist Management System is a full-stack web application designed to streamline tour package browsing, booking, and administrative management.
Users can explore curated travel packages, register accounts, and purchase tours online. The system features a centralized administrator dashboard that enables travel managers to control package offerings, monitor registered users, and track payment transactions.
The platform includes user authentication, package catalog management, an automated purchase workflow, payment logging, and database-driven data persistence.

✨ Features

👤 User Features
User registration and login
Session-based authentication & secure logout
Browse available tour packages
View package details, schedules, and pricing
Purchase and book tour packages
View purchasing history and account details
Responsive layout for mobile and desktop browsing

🌴 Tour & Booking System
Catalog of travel packages
Package image gallery
Direct online package purchasing
Automated booking transaction processing
Dynamic package pricing display

🛡️ Admin Features
Dedicated administrator dashboard
System-wide overview and activity metrics
Package Management:
  Add new tour packages
  Edit package details and pricing
  Delete obsolete packages
User Management:
  View all registered users
  Update user information and access
Payment History:
  Track customer purchases
  Review payment logs and transaction history

🏗️ Project Structure

Tourist-Management-System-main/
│
├── admin/
│   ├── dashboard.php
│   ├── manage_packages.php
│   ├── manage_packages_section.php
│   ├── manage_users.php
│   ├── manage_users_section.php
│   ├── payment_history_section.php
│   └── update_user.php
│
├── images/
│   ├── nico-smit-uT3K66fLWK8-unsplash.jpg
│   ├── sudhanshu-yadav-ADUi7T5FdX8-unsplash.jpg
│   └── t1.jpg
│
├── includes/
│   ├── db.php
│   ├── footer.php
│   ├── functions.php
│   └── navbar.php
│
├── sql/
│   └── database.sql
│
├── index.php
├── login.php
├── logout.php
├── packages.php
├── purchase.php
├── register.php
└── s.css

🛠️ Technologies Used

Technology           Purpose
---------------------------------------------------------------------
PHP                  Server-side application logic and backend processing
MySQL                Database management and relational data storage
HTML5                Page structure and semantic markup
CSS3                 Custom styling, layout, and visual presentation
Apache               Local web server environment (XAMPP / WAMP)
Git & GitHub         Version control and repository management

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
       │ & Confirmation│
       └───────────────┘

🚀 Getting Started

Prerequisites
Make sure you have the following installed:
* XAMPP (or any local Apache + MySQL stack)
* PHP 7.4+ or 8.+
* MySQL / MariaDB
* Web browser (Chrome, Firefox, Edge, etc.)

1. Clone the Repository
git clone https://github.com/Iftekharul756/Tourist_Management_System_DBMS.git

2. Move to Local Server Directory
Copy or move the cloned folder inside your local web server root directory:
C:\xampp\htdocs\Tourist-Management-System-main\

3. Start Apache & MySQL
Launch the XAMPP Control Panel and start both Apache and MySQL services.

4. Import the Database
1. Open phpMyAdmin in your browser: http://localhost/phpmyadmin/
2. Create a new database (e.g., `tourist_management` or match the name in `includes/db.php`).
3. Select the newly created database and click the Import tab.
4. Choose the file located at: `sql/database.sql`
5. Click Go to execute the SQL script and build the tables.

5. Verify Database Credentials
Open `includes/db.php` and verify that the database credentials match your local setup:
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "tourist_management";

6. Run the Application
Open your web browser and visit:
http://localhost/Tourist-Management-System-main/index.php

🔐 User Roles

Customer / User
* Account registration and login
* View catalog of tour packages
* Access package details
* Purchase packages
* View individual booking/purchase records

Administrator
* Access the admin panel (`/admin/dashboard.php`)
* Add, edit, and delete tour packages
* Manage registered user accounts
* Review payment histories and transaction logs

📚 Key Development Concepts

This project demonstrates practical experience with:
* Full-stack PHP & MySQL web development
* Relational Database Management Systems (DBMS)
* User session authentication and authorization
* CRUD (Create, Read, Update, Delete) data operations
* Form handling and backend validation
* Modular PHP file organization (`includes/` and `admin/`)
* Relational schema design and SQL scripting
* Version control workflows with Git and GitHub

👨‍💻 Author

Md Iftekharul Alam
B.Sc. in Computer Science & Engineering
Interested in Artificial Intelligence, Machine Learning, Data, and Software Development.

⭐ Support

If you find this project helpful, consider giving the repository a ⭐!
