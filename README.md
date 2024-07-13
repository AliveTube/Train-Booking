# Train Booking Application

## Description
This C# console application simulates a train booking system with functionalities for user registration, login for both customers and administrators, and various administrative tasks like adding trains, managing trips, and adding new administrators. It interacts with a SQL Server database (`projectDB`) for data storage and retrieval.

## Features
- **User Management**:
  - Register as a customer with first name, last name, email, password, and phone number.
  - Login as a customer or admin.
  - Edit customer and admin profiles.

- **Administrator Features**:
  - **Add Train**: Add details of a new train to the system.
  - **Edit Train Details**: Modify existing train information.
  - **Add Trip**: Schedule a new trip including associated train details.
  - **Edit Trip Details**: Modify existing trip schedules.
  - **Add New Admin**: Register a new administrator to manage the system.

- **Customer Features**:
  - **Book a Ticket**: Reserve seats on available trips.
  - **List All Trips**: Display all scheduled trips.

## Dependencies
- Microsoft .NET Framework
- SQL Server (or SQL Server Express) for database operations

## Setup Instructions
1. **Database Setup**:
   - Ensure SQL Server is installed and running.
   - Create a database named `projectDB`.

2. **Connection Configuration**:
   - Modify the connection strings in the application (`Main` method) to match your SQL Server instance and database (`Data Source`, `Initial Catalog`, `Integrated Security`).

3. **Compilation and Execution**:
   - Compile the `Program.cs` file using Visual Studio or `csc` command line tool.
   - Execute the compiled program to start the application.

## Usage
1. Run the application.
2. Choose an option from the main menu:
   - Register as a new customer (`1`).
   - Login as an admin (`2`) or customer (`2`).
   - Exit the application (`3`).

3. Follow on-screen prompts to perform desired actions like adding trains, scheduling trips, booking tickets, or managing user profiles.

## Example
```
Welcome to Train Booking application 

Please choose one of the following
1- Register
2- Login
3- Exit
1

Please enter the following credentials
First name : Belal
Last name : Ahmed
Email : bebobale@gmail.com
Password : ******
Phone Number : +123456789

You have been registered successfully :)
Your ID is: 123

Choose one of the following :
1- Login as an admin
2- Login as a customer
3- Return to main menu
2

Please enter the following credentials
Customer ID : 123
Password : ******
Welcome back Belal Ahmed

Choose one of the following :
1- Book a ticket
2- List all trips
3- Return to main menu
```
