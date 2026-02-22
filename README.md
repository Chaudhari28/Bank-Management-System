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






