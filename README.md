# Student Database Management System

## Overview

The **Student Database Management System (SDMS)** is a robust and secure solution for managing and maintaining student data. Designed using C++ programming language, the system interacts with a MySQL relational database management system (RDBMS) to handle various database operations like viewing, editing, and updating records. The system is structured using object-oriented programming (OOP) principles to ensure clean and modular code. It incorporates key features such as multi-threading, encryption, and decryption to ensure data security and efficient operation.

This project is intended to demonstrate the application of advanced programming concepts, database management, and security in a real-world scenario. The goal is to provide a scalable system that can be used by educational institutions for managing student information securely and efficiently.

## Key Features

- **User-based Views:** Different user types (e.g., Admin, Student, Faculty) can access the database with tailored views and permissions.
- **CRUD Operations:** Support for Create, Read, Update, and Delete operations on student data.
- **Data Security:** Implements encryption and decryption mechanisms to secure sensitive data.
- **Multi-threading:** Optimized performance with multi-threaded operations to handle large-scale data.
- **Database Integration:** MySQL used as the database backend to store student records.
- **Role-based Access Control (RBAC):** Restrict user actions based on roles to ensure that only authorized users can modify data.

## Technologies Used

- **C++:** Core programming language used for developing the system logic and database interaction.
- **MySQL:** Relational Database Management System (RDBMS) used for storing student data.
- **Object-Oriented Programming (OOP):** The project follows OOP principles for modular and reusable code design.
- **Data Structures:** Efficient data structures are used for data storage and retrieval.
- **Multi-threading:** Optimized the system to handle multiple requests simultaneously.
- **Encryption/Decryption:** AES or similar encryption algorithms are implemented to protect sensitive student data.
- **Git/GitHub:** Version control to manage project updates and collaboration.

## Installation

### Prerequisites

- C++ Compiler (e.g., GCC, Clang)
- MySQL Database Server
- OpenSSL or other libraries for encryption/decryption
- CMake (for building the project)
  
### Steps to Set Up

1. **Clone the Repository:**


2. **Install Dependencies:**
- Install MySQL server and set up a database.
- Install C++ compiler and libraries for multi-threading and encryption.

3. **Set Up Database:**
- Create a MySQL database and tables based on the schema provided in the `database_schema.sql` file.
- Configure database credentials in the application’s configuration file.

4. **Build the Project:**
- Navigate to the project directory.
- Run CMake to generate build files:
  ```
  mkdir build
  cd build
  cmake ..
  make
  ```

5. **Run the System:**
- After building, run the executable:
  ```
  ./student_database_system
  ```

## Project Structure


## Security Features

This project focuses heavily on data security, especially when handling sensitive student information. The system implements:

- **AES Encryption:** Sensitive fields like student personal information and grades are encrypted using AES encryption before being stored in the database.
- **Decryption on Access:** Only authorized users can decrypt and view the sensitive data.
- **Role-based Access Control (RBAC):** Permissions are based on the role of the user, ensuring data is accessed only by those authorized.

## How to Use

1. **Login:** Users must log in with their credentials (username and password). The system supports multiple user roles, each with specific permissions.
2. **Database Interaction:** After login, users can perform CRUD operations based on their role.
3. **Security:** The system encrypts sensitive data before storing it in the database. When viewing or updating this data, proper decryption will be handled automatically by the system.

## Future Enhancements

- **User Authentication:** Implement advanced authentication mechanisms such as two-factor authentication (2FA).
- **Data Visualization:** Add a module for generating reports or graphs based on student data.
- **Backup/Restore:** Implement a backup and restore feature to ensure data safety.

## Contributing

Feel free to fork this repository and contribute by submitting pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or suggestions, please reach out to [Your Name] at [your.email@example.com].

