# Employee Management System

The Employee Management System is a Python application that allows users to manage employee records efficiently. This system provides features for adding, updating, deleting, and searching for employee information. It uses a MySQL database to store and retrieve data.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Database Setup](#database-setup)
- [Application Screenshots](#application-screenshots)


## Features

- Add new employee records, including details like name, department, email, and more.
- Update existing employee information.
- Delete employee records.
- Search for employees by various criteria, such as phone number or ID proof.
- Display employee records in a user-friendly table format.

## Requirements

To run this application, you'll need the following:

- Python 3.x installed on your system.
- The following Python libraries: tkinter, mysql.connector, and Pillow (for image handling).
- Access to a MySQL database.

## Installation

1. Clone or download the project repository to your local machine.

   ```
   git clone https://github.com/your-username/employee-management-system.git
   ```

2. Install the required Python libraries using pip.

   ```
   pip install tkinter mysql-connector-python pillow
   ```

## Usage

1. Ensure that you have set up a MySQL database for the application.

2. Modify the script to include your database credentials and any other necessary configurations.

3. Run the application.

   ```
   python employee_management.py
   ```

4. Use the application to manage employee records.

## Database Setup

To set up the MySQL database for this application, follow these steps:

1. Create a new MySQL database.

2. Define a table named `emp` with appropriate columns to store employee information. You can use the following SQL command as a reference:

   ```sql
   CREATE TABLE emp (
       id INT AUTO_INCREMENT PRIMARY KEY,
       Department VARCHAR(255),
       Name VARCHAR(255),
       Designation VARCHAR(255),
       Email VARCHAR(255),
       Address VARCHAR(255),
       Married_Status VARCHAR(255),
       DOB DATE,
       DOJ DATE,
       ID_Proof_Type VARCHAR(255),
       ID_Proof VARCHAR(255) UNIQUE,
       Gender VARCHAR(255),
       Phone VARCHAR(15),
       Country VARCHAR(255),
       Salary DECIMAL(10, 2)
   );
   ```

3. Update the database connection details in the Python script to match your MySQL setup.

## Application Screenshots

![Screenshot 2023-09-02 225542](https://github.com/Harshit3726/Employee-Management-System/assets/117848999/a4ebdedb-0cf2-462d-82f7-f34c5c9d4330)

