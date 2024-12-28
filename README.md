# Simple CRUD Mahasiswa (PHP)

This repository demonstrates a simple CRUD (Create, Read, Update, Delete) application for managing mahasiswa (student) data using PHP. The project is straightforward, making it ideal for beginners learning PHP and database integration.

## Features
- Add new student records.
- View a list of students.
- Update existing student records.
- Delete student records.

## Prerequisites
- PHP 7.4 or later.
- A web server (e.g., Apache or Nginx).
- MySQL or another compatible database system.
- A web browser to access the application.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/dzikrimaulana87/simple_crud_mahasiswa-php.git
   cd simple_crud_mahasiswa-php
   ```

2. **Set Up the Database**
   - Import the `database.sql` file into your MySQL database.
     ```sql
     mysql -u your_username -p your_database_name < database.sql
     ```
   - Update the database connection settings in the `koneksi.php` file:
     ```php
     <?php
     $host = 'localhost';
     $user = 'your_username';
     $pass = 'your_password';
     $db   = 'your_database_name';

     $conn = mysqli_connect($host, $user, $pass, $db);
     if (!$conn) {
         die('Connection failed: ' . mysqli_connect_error());
     }
     ?>
     ```

3. **Deploy the Application**
   - Place the project files in your web server's root directory (e.g., `htdocs` for XAMPP).
   - Start your web server and navigate to the application in your browser:
     ```
     http://localhost/simple_crud_mahasiswa-php
     ```

## File Structure
- `index.php`: Main page listing all students.
- `tambah.php`: Page for adding new student records.
- `edit.php`: Page for updating existing student records.
- `hapus.php`: Handles deleting student records.
- `koneksi.php`: Database connection file.
- `database.sql`: SQL script for setting up the database.

## Usage
1. Navigate to the application in your web browser.
2. Use the navigation links to add, edit, or delete student records.

## Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.

---

For issues or questions, please open an issue on the repository or contact [me](https://www.linkedin.com/in/dzikrimaulana87/).
