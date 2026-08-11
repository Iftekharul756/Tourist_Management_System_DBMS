# Tourist Management System – Travel & DBMS Platform

A web-based **Tourist Management System** developed using **PHP and MySQL** to manage tour packages, user accounts, bookings, and payment records.

The system provides a simple platform for users to browse and purchase tour packages, while administrators can manage packages, registered users, and payment information through a dedicated admin panel.

---

## 📌 Overview

The **Tourist Management System** is a database-driven web application designed to demonstrate the practical implementation of **PHP, MySQL, and DBMS concepts** in a travel management environment.

Users can create accounts, log in, explore available tour packages, and purchase packages. Administrators have access to a separate dashboard for managing tour packages, user accounts, and payment records.

---

## ✨ Features

### 👤 User Features

* User registration and login
* Session-based authentication and logout
* Browse available tour packages
* View package details and prices
* Purchase tour packages
* Access account and booking information

### 🛡️ Admin Features

* Dedicated administrator dashboard
* **Package Management** – Add, edit, and delete tour packages
* **User Management** – View and manage registered users
* **Payment History** – View and track user purchase records

---

## 🏗️ Project Structure

```text
Tourist-Management-System-main/
│
├── admin/                         # Admin dashboard and management scripts
│   ├── dashboard.php
│   ├── manage_packages.php
│   ├── manage_packages_section.php
│   ├── manage_users.php
│   ├── manage_users_section.php
│   ├── payment_history_section.php
│   └── update_user.php
│
├── images/                        # Project image assets
│
├── includes/                      # Database connection and shared components
│   ├── db.php
│   ├── footer.php
│   ├── functions.php
│   └── navbar.php
│
├── sql/                           # Database schema
│   └── database.sql
│
├── index.php                      # Homepage
├── login.php                      # User login
├── logout.php                     # Logout handler
├── packages.php                   # Tour packages
├── purchase.php                   # Package purchase handler
├── register.php                   # User registration
└── s.css                          # Custom stylesheet
```

---

## 🛠️ Technologies Used

| Technology          | Purpose                                   |
| ------------------- | ----------------------------------------- |
| **PHP**             | Backend development and application logic |
| **HTML5**           | Page structure                            |
| **CSS3**            | Styling and layout                        |
| **JavaScript**      | Client-side functionality                 |
| **MySQL / MariaDB** | Database management                       |
| **Apache**          | Local web server                          |
| **XAMPP / WAMP**    | Local development environment             |
| **Git & GitHub**    | Version control                           |

---

## 🔄 Application Workflow

```text
                    ┌───────────────────┐
                    │     Register      │
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
                ┌─────────────┴─────────────┐
                │                           │
                ▼                           ▼
       ┌─────────────────┐        ┌─────────────────┐
       │ Browse Packages │        │   Admin Panel   │
       └────────┬────────┘        └────────┬────────┘
                │                          │
                ▼                          ▼
       ┌─────────────────┐        ┌─────────────────┐
       │ Purchase Package│        │ Manage Packages │
       └────────┬────────┘        │ & Users         │
                │                 │                 │
                ▼                 │ Payment History │
       ┌─────────────────┐        └─────────────────┘
       │ Payment Record  │
       └─────────────────┘
```

---

## 🚀 Getting Started

### Prerequisites

Make sure the following are installed:

* **XAMPP** or another local Apache + MySQL environment
* **PHP 7.4+** or PHP 8.x
* A modern web browser
* **Git** (optional, for cloning the repository)

### 1. Clone the Repository

```bash
git clone https://github.com/Iftekharul756/Tourist_Management_System_DBMS.git
```

### 2. Move the Project to the Server Directory

Copy the project folder into your local web server's root directory.

For XAMPP:

```text
C:\xampp\htdocs\Tourist-Management-System-main
```

### 3. Start Apache and MySQL

Open the **XAMPP Control Panel** and start:

* Apache
* MySQL

### 4. Set Up the Database

Open phpMyAdmin:

```text
http://localhost/phpmyadmin/
```

Create a new database named:

```text
tourist_management
```

Then:

1. Select the `tourist_management` database.
2. Open the **Import** tab.
3. Select `sql/database.sql` from the project.
4. Click **Go** to import the database.

### 5. Verify the Database Connection

Open:

```text
includes/db.php
```

Make sure the database configuration matches your local MySQL setup:

```php
$servername = "localhost";
$username = "root";
$password = "";
$dbname = "tourist_management";
```

> If your MySQL installation uses a different username, password, or port, update the configuration accordingly.

### 6. Run the Application

Open your browser and visit:

```text
http://localhost/Tourist-Management-System-main/index.php
```

The application should now be running locally.

---

## 🔐 User Roles

### Customer / User

Users can:

* Create an account
* Log in and log out
* Browse available tour packages
* Purchase tour packages
* Access booking/account information

### Administrator

Administrators can:

* Access the admin dashboard
* Add, edit, and delete tour packages
* Manage registered users
* View payment histories

Admin panel:

```text
/admin/dashboard.php
```

---

## 📚 Key Concepts Demonstrated

This project demonstrates several practical concepts in web development and database management:

* PHP-based web application development
* MySQL relational database management
* Database-driven application design
* Session-based authentication
* User authorization and role management
* CRUD operations
* Form handling and validation
* PHP–MySQL database integration
* Git and GitHub version control

---

## 👨‍💻 Author

**Md Iftekharul Alam**
B.Sc. in Computer Science & Engineering

Interested in **Artificial Intelligence, Machine Learning, Data, and Software Development**.

---

## ⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.
