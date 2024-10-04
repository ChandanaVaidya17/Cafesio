# Cafesio
Cafesio is a web-based cafe management system designed for online food ordering and order tracking. Built using PHP, MySQL, HTML, and CSS, Cafesio provides an intuitive interface for both admins and users.
## Features

### For Admins
- Manage food items: Add, update, or delete food items and their properties.
- View and track all incoming orders.
- Update the status of orders (e.g., processing, completed, or canceled).

### For Users
- Browse the menu and view details of food items.
- Place orders for selected food items and specify the quantity.
- Track the status of their orders in real-time.

## Technologies Used
- **Frontend**: HTML, CSS
- **Backend**: PHP
- **Database**: MySQL

## Installation
1. **Clone the Repository**
   ```bash
   git clone https://github.com/ChandanaVaidya17/Cafesio.git
   ```
2. **Set Up the Database**
   - Create a MySQL database and import the provided `cafesio.sql` file.
   - Update the `config.php` file with your database credentials.

3. **Configure the Environment**
   - Make sure your server is running PHP and MySQL.
   - Place the project files in your web server's root directory (e.g., `htdocs` for XAMPP).
4. **Access the Application**
   - Open your web browser and navigate to `http://localhost/cafesio` to start using the application.

## Configuration

- **Database Configuration**: Edit `config.php` to set your database host, username, password, and database name.
  ```php
  <?php
  $host = 'localhost'; // Database host
  $user = 'root';      // Database username
  $password = '';      // Database password
  $dbname = 'cafesio'; // Database name
  
  // Create connection
  $conn = new mysqli($host, $user, $password, $dbname);
  
  // Check connection
  if ($conn->connect_error) {
      die("Connection failed: " . $conn->connect_error);
  }
  ?>
  ```
## Usage

- **Admin Login**: Access the admin dashboard by logging in with the admin credentials provided during setup.
- **User Login**: Users can create accounts and log in to place and track orders.

