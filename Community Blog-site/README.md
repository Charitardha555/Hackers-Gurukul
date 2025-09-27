
# Blog Application

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview
This Blog Application is a comprehensive platform built with PHP, MySQL, HTML, CSS, and JavaScript, designed to allow users to create, edit, and manage blog posts with rich multimedia content. It supports user authentication with role-based access control (Admin, Mentor, Student), ensuring secure and structured content management. The application features a responsive and intuitive UI suitable for both desktop and mobile devices.

## Features
- User Registration and Secure Login with Password Hashing  
- Role-Based Access Control  
  - Admin: Full control over users, posts, and comments  
  - Mentor: Can create, edit, and manage posts and comments  
  - Student: Can create posts and comment  
- Post Creation with Media Upload (images/videos)  
- Commenting System on Posts  
- Search Functionality for Posts by Title or Content  
- User Profile with Avatar Management  
- Admin Dashboard with User, Post, and Comment Moderation  
- Responsive Design using Bootstrap  

## Technologies Used
- **Backend:** PHP (Object-Oriented Programming)  
- **Frontend:** HTML5, CSS3, JavaScript, Bootstrap 5  
- **Database:** MySQL  
- **Server Environment:** Apache on XAMPP/WAMP/LAMP  

## Installation

### Prerequisites
- Web server (Apache) with PHP support  
- MySQL or MariaDB database server  
- PHP 7.4+ recommended  
- Local server environment recommended: [XAMPP](https://www.apachefriends.org/index.html)  
https://github.com/Charitardha555/Hackers-Gurukul/tree/02ab4a128b20d70c5e949d15166c2abd6b802926/Community%20Blog-site

2. **Import the database schema**  
- Open your MySQL client (phpMyAdmin, MySQL CLI)  
- Import the `blog_app.sql` file located in the `/database` folder  
3. **Configure database connection**  
- Open `db_connection.php`  
- Update the following variables with your database credentials:  
  ```
  $dbHost = 'localhost';
  $dbUser = 'root';
  $dbPass = '';
  $dbName = 'blog_application';
  ```  
4. **Set up the project directory**  
- Place the project folder inside your web server’s root directory (e.g., `htdocs` for XAMPP)  
5. **Run the application**  
- Open your browser and navigate to `http://localhost/blog-application`  
6. **Create your first user**  
- Register via the registration page or set an admin user directly in the database  

## Usage
- Register, login, and select your role during registration (if applicable)  
- Create new posts using the dashboard  
- Upload images or videos embedded within your posts  
- Comment on posts and interact with other users  
- Admin users can manage all users, posts, and comments  
- Use the search bar to quickly find specific content  

## Folder Structure
blog-application/
│
├── assets/ # CSS, JavaScript, images, fonts
├── config.php # Database config and global settings
├── index.php # Home page - list of blog posts
├── login.php # Login page
├── register.php # User registration page
├── logout.php # Logout script
├── post/ # Create, edit, delete posts scripts
├── comments/ # Manage comments scripts
├── admin/ # Admin panel dashboard and management
├── database/ # Database schema and seed files
├── README.md # Project README file
└── .gitignore # Git ignore file

---

Thank you for using this Blog Application! Your feedback and contributions are highly appreciated.

### Steps
1. **Clone the repository**  
