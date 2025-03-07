Banking-System
Overview:
This is a simple Banking System implemented in Java with Oracle Database. It allows users to add, view, and delete bank accounts using a console-based interface. The system connects to an Oracle database using JDBC for data management.
Features:
Add Bank Account -Users can create new bank accounts by entering the account holder's name and initial balance.
View All Accounts – Displays all bank accounts stored in the database.
Delete Account – Removes an account from the database using the account ID.

Database Schema
The system uses a table named BankAccount with the following structure:
Technologies Used
Java (JDBC for database connectivity)
Oracle Database (SQL for data storage)
Eclipse (or any IDE for Java development)

Setup Instructions:
1.Ensure Oracle Database is installed and running.
2.Create the BankAccount table using the following SQL query:

CREATE TABLE BankAccount (
    account_id NUMBER GENERATED ALWAYS AS IDENTITY PRIMARY KEY,
    account_holder_name VARCHAR2(100) NOT NULL,
    account_balance NUMBER(10,2) NOT NULL);

3.Update database connection details in the OracleDatabaseConnection.java file.
4. Run the Java program from your IDE or command line.

Usage:
Run the program and select an option from the menu.
Follow the prompts to add, view, or delete bank accounts.

Notes
Make sure the database connection is properly configured.
The program assumes a valid Oracle Database is available.
The delete option requires entering a valid account ID.

Future Improvements:

1. Implement update account balance functionality.
2. Add transaction history tracking for deposits and withdrawals.
3. Improve error handling for invalid inputs.
