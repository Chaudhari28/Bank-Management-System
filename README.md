# Bank-Management-System
Bank Management System is a Java Swing and AWT desktop app that simulates core banking operations. It offers secure login, account management, deposits, withdrawals, balance inquiry, and mini statements, showcasing OOP concepts with a simple, user‑friendly GUI.
The Bank Management System is a desktop application built using Java Swing and AWT. It provides a simple, interactive interface that simulates core banking operations such as account login, PIN authentication, and transaction handling. This project demonstrates how Java can be used to design a structured, user-friendly system for managing basic banking workflows.
Features
- 🔐 Secure Login with Card Number and PIN
- 🏦 Account Management: Create and manage customer accounts
- 💳 ATM Operations: Deposit, Withdraw, Balance Inquiry
- 📊 Mini Statement: View recent transactions
- 🎨 Graphical User Interface (GUI) using Swing and AWT

Technologies Used
- Java (Core + Swing + AWT)
- Object-Oriented Programming (OOP) concepts
- File Handling / Database (optional) for storing user data

🔑 Login Page (Java Swing & AWT)
- Entry Point: Acts as the gateway to the Bank Management System.
- Secure Authentication: Users enter Card Number and PIN to access services.
- Input Fields: Text field for card number and password field for PIN (hidden input).
- Action Buttons: Includes Sign In for authentication, with options for future expansion (Clear, Sign Up).
- User Interface: Designed with Swing and AWT, featuring labels, styled fonts, and background graphics for an ATM‑like look.
- Error Handling: Can be extended to validate incorrect credentials and display messages.
- Scalability: Serves as the foundation for connecting to account management and transaction modules.

Screenshot
<img width="1061" height="625" alt="image" src="https://github.com/user-attachments/assets/4836c36c-1afc-4736-9af5-5f6d51429f07" />

🏦 Signup Form (Java Swing)
📌 How This Page Came About
- Started as part of a Bank Management System project to simulate real-world banking workflows.
- The Signup Page (Page 1) was designed to collect personal details from users before account creation.
- Built using Java Swing for GUI because it’s lightweight, flexible, and widely used for desktop applications.
- Added JDateChooser (from the Toedter library) to provide a user-friendly calendar for selecting Date of Birth.
- Used Random class to generate a unique Application Form Number for each new applicant.
- Applied custom styling (fonts, colors, icons) to make the form look professional and visually appealing.
- Implemented radio buttons for Gender and Marital Status to ensure clean, mutually exclusive selections.
- Added a Next button with ActionListener to prepare for navigation to subsequent pages (future expansion).

📌 How It Works
- When you run Signup.java, the application window opens with the Bank icon and a randomly generated form number.
- Users fill in their details: name, father’s name, DOB, gender, email, marital status, address, city, pin code, and state.
- The Date Picker allows easy selection of DOB instead of manual typing.
- Radio buttons ensure only one option can be selected for gender and marital status.
- Clicking Next will trigger the actionPerformed() method, where future logic (like saving to a database or moving to Page 2) can be added.

Screenshot
<img width="1070" height="990" alt="image" src="https://github.com/user-attachments/assets/80896c0b-a2ff-4cb7-91d3-506e03ce61c1" />

🚀 What’s Next
- Database Integration: Connect the Signup form with a MySQL database using JDBC.
- Table Creation: Design tables to store user details (Name, DOB, Gender, Email, Marital Status, Address, City, Pin code, State).
- Data Insertion: Write SQL queries to insert form data into the database when the user clicks Next.
- Navigation: Extend the Next button functionality to move to Page 2 after saving Page 1 details.
- Validation: Add input checks (e.g., email format, pin code length) before saving data.
- Scalability: Prepare the project for multi-page forms and complete account creation workflow.

🏦 Bank Management System – Signup Module (Java + MySQL)
This project is a Bank Management System Signup Module developed using Java Swing for the frontend and MySQL for the backend database.
📌 Features
User-friendly Application Form (Page 1) GUI
Collects personal details:
-Name
-Father’s Name
-Date of Birth
-Gender
-Email
-Marital Status
-Address
-City
-Pincode
-State
-Auto-generates a unique Application Form Number
-Stores user data into MySQL database
-Navigates to next page (Signup2) after successful submission

🛠️ Technologies Used
Java (Swing & AWT) – GUI Development
-MySQL – Database
-JDBC – Database Connectivity
-JCalendar (JDateChooser) – Date Picker

🗄️ Database
-Database Name: bankSystem
-Table Name: signup
-Stores all applicant details submitted through the form.

📂 Project Structure
-Signup.java → Main application form
-Signup2.java → Next page of form
-Con.java → Database connection class

Screenshot
<img width="1073" height="128" alt="image" src="https://github.com/user-attachments/assets/c2f0d2e5-9dcd-4763-91e5-e9939095be9d" />

📌 Signup Page 2 – Additional Details
This is the second page of the account opening form in my Bank Management System project built using Java Swing.
🔹Features Implemented
Dropdown selections for:
-Religion
-Category
-Income
-Educational Qualification
-Occupation
-Input fields for:
-PAN Number
-Aadhar Number
-Radio button selections for:
-Senior Citizen (Yes/No)
-Existing Account (Yes/No)
-Dynamic Form Number display
-Custom UI styling using Java Swing components
-Bank logo integration
-Navigation button to proceed to the next page

Screenshot
<img width="1044" height="917" alt="image" src="https://github.com/user-attachments/assets/9819e08c-a96c-46d4-9645-42a39987fe40" />

📌Signup Page 3 – Account Details Module
This module is part of my Bank Management System project built using Java (Swing) and MySQL.
✅Features Implemented:
-Account Type selection
-Saving Account
-Fixed Deposit
-Current Account
-Recurring Deposit Account
-Auto-generated Card Number (16-digit format)
-Auto-generated 4-digit PIN
-Banking Services Selection:
-ATM Card
-Internet Banking
-Mobile Banking
-Email Alerts
-Check Book
-E-Statement
-Declaration Checkbox
-Submit & Cancel functionality

Screenshot
<img width="1038" height="987" alt="image" src="https://github.com/user-attachments/assets/49aec771-0d5b-4468-a36a-2ff566aaa147" />

📌Database creation for signupthree page and login page
Today I implemented the database structure for the final step of account creation in the Bank Management System built with Java, Swing, and MySQL.
Tables Created

1. signupthree
This table stores the final account details selected by the user during registration.

Fields included:
form_no – unique form number of the applicant
account_type – type of bank account (Saving / Current / etc.)
card_number – generated ATM card number
pin – user PIN for ATM/login
facility – selected banking facilities (ATM card, Internet banking, etc.)

SQL

create table signupthree(
form_no varchar(30),
account_type varchar(40),
card_number varchar(30),
pin varchar(30),
facility varchar(200)
);
<img width="625" height="125" alt="image" src="https://github.com/user-attachments/assets/bb75f44d-ded6-4a33-b12a-0e62637c1c7e" />

2. login
This table is used for authentication in the banking system.

Fields included:
form_no
card_number
pin

SQL

create table login(
form_no varchar(30),
card_number varchar(50),
pin varchar(30)
);
<img width="604" height="142" alt="image" src="https://github.com/user-attachments/assets/adf2a841-7e81-4a68-aaa7-b1491f654680" />

Purpose

These tables allow the system to:
Store the user's final account details
Generate ATM card and PIN
Enable secure login to the banking system

📌Deposit Module
This project is part of a Java-based Bank Management System that simulates an ATM interface. The Deposit module allows users to enter an amount and store the transaction securely in a database.

Features
-ATM-style graphical interface built using Java Swing
-Deposit amount input system
-Transaction recording with PIN, Date, Type, and Amount
-MySQL database integration
-Instant confirmation message after successful deposit

Screenshot:
<img width="1886" height="1019" alt="image" src="https://github.com/user-attachments/assets/ae51f5c8-7f8e-4ef0-933e-a5032ccc03e1" />

Database Structure:
<img width="917" height="172" alt="image" src="https://github.com/user-attachments/assets/2e256da6-7aa7-440d-9d2e-f2b84f7a1c98" />

📌Withdrawal and BalanceEnquiry
-Implemented the Withdrawal module where users can enter an amount and withdraw money from their account.
-Before processing the withdrawal, the system checks the user’s current balance by reading all previous transactions from the database.
-If the balance is sufficient, the withdrawal transaction is recorded in the bank table with the user’s PIN, date, transaction type, and amount.
-Added validation to prevent withdrawals when the balance is insufficient.
-Implemented the Balance Enquiry feature that calculates the user’s current balance.
-The system loops through all deposit and withdrawal records related to the user’s PIN and calculates the final balance dynamically.
-The calculated balance is then displayed on the ATM interface using Java Swing.
-Used JDBC to connect Java with MySQL for storing and retrieving transaction data.
-Implemented button event handling for actions like Withdraw and Back to navigate between ATM screens.

Screenshot:
<img width="1060" height="596" alt="image" src="https://github.com/user-attachments/assets/3fe0105f-550b-4825-9031-3d5a3c04eaae" />
<img width="1528" height="980" alt="image" src="https://github.com/user-attachments/assets/6b0e1f6f-155c-4bb4-84d4-1006f6bff092" />
<img width="1528" height="973" alt="image" src="https://github.com/user-attachments/assets/cca480c3-b98e-4031-93df-d9307d99373d" />
<img width="1530" height="980" alt="image" src="https://github.com/user-attachments/assets/884cd652-a94c-4f55-bb82-bb934c7669eb" />

SQL:
<img width="885" height="252" alt="image" src="https://github.com/user-attachments/assets/c8303f5c-48df-40f9-a7aa-9623c863e153" />


