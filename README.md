# Online Recipe Collection System

## Overview

The Online Recipe Collection System is a web-based application that allows **Admins** to manage recipes and **Users** to browse, search, and review them. The system supports user authentication, review submission, and recipe management via a MySQL database.

![Online Recipe Screenshot](https://raw.githubusercontent.com/Ilmaa2003/Online-Recipe-Collection/main/Images/IMG-20250619-WA0028.jpg)

![Online Recipe Screenshot](https://raw.githubusercontent.com/Ilmaa2003/Online-Recipe-Collection/main/Images/IMG-20250619-WA0025.jpg)

![Online Recipe Screenshot](https://raw.githubusercontent.com/Ilmaa2003/Online-Recipe-Collection/main/Images/IMG-20250619-WA0023.jpg)

---

## Features

### Admin

- Secure admin login
- Add, edit, delete, and view recipes
- Manage recipe details: title, ingredients, instructions, category, and images

### User

- User registration and login
- Browse and search recipes by category or keywords
- View detailed recipe information
- Submit reviews or comments on individual recipes
- View reviews submitted by other users

---

## Technologies Used

| Layer      | Technology         |
|------------|--------------------|
| Frontend   | HTML, CSS, JavaScript |
| Backend    | PHP                |
| Database   | MySQL              |
| Tools      | Visual Studio Code, XAMPP, phpMyAdmin |

---

## Development Tools and Setup

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/)
- [XAMPP (Apache + PHP + MySQL)](https://www.apachefriends.org/download.html)
- [PHP Server Extension](https://marketplace.visualstudio.com/items?itemName=brapifra.phpserver)
- [PHP IntelliSense Extension](https://marketplace.visualstudio.com/items?itemName=felixfbecker.php-intellisense)

---

## Setup Instructions

### Step 1: Install Software

1. **Install Visual Studio Code**  
   Download and install from: [https://code.visualstudio.com/](https://code.visualstudio.com/)

2. **Install XAMPP**  
   Download from: [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html)  
   Follow installation instructions to set up Apache and MySQL.

3. **Install PHP Extensions in VS Code**  
   - Open VS Code  
   - Go to Extensions (`Ctrl+Shift+X`)  
   - Install the following:
     - **PHP Server**: For running PHP locally
     - **PHP IntelliSense**: For intelligent code suggestions

---

### Step 2: Project Setup

1. **Move your project folder** to the XAMPP web directory:
```

C:\xampp\htdocs\your\_project\_folder\\

````

2. **Start Apache and MySQL** via XAMPP Control Panel:
- Open XAMPP Control Panel
- Click **Start** next to both **Apache** and **MySQL**
- Ensure both services are running (green indicators)

3. **Create the database** using phpMyAdmin:
- Open a browser and go to: `http://localhost/phpmyadmin/`
- Create a new database (e.g., `recipe_system`)
- Import the provided SQL file if available or manually create tables

4. **Configure database connection** in your PHP config file (e.g., `config.php`):
```php
$host = "localhost";
$username = "root";
$password = "";
$database = "recipe_system";
$conn = new mysqli($host, $username, $password, $database);
```

5. **Run the application**

   * Open your browser and visit:

     ```
     http://localhost/your_project_folder/
     ```

-----

## You're All Set!

You can now develop, test, and enhance your PHP-based recipe collection system using Visual Studio Code and XAMPP.


