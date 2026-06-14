# Wallet_X-
WalletX Pro is a full-stack financial dashboard designed to simulate a modern mobile money application. The project focuses on relational database design, secure transaction handling, and business intelligence reporting.

🚀 Key Features
User Onboarding: Dynamic registration with validation.
P2P Transfers: Secure money transfers between users using SQL Transaction logic.
Bill Payments: Integrated system to pay utilities (LESCO, PTCL, etc.).
BI Dashboard: Real-time metrics for Active Users, Total Liquidity, and Revenue Charts.
Admin Search: Multi-filter search for user account management.
🛠 Tech Stack
Frontend: Streamlit (Python-based Web Framework)
Database: Microsoft SQL Server (MS SQL)
Data Analysis: Pandas
Visualization: Plotly Express
Driver: pyodbc for Python-to-SQL connectivity
📂 Database Setup
This repository includes a .sql file containing the schema and dummy data.
Open SQL Server Management Studio (SSMS).
Create a new database named WalletX.
Open the provided database_schema.sql (or whatever your file name is) and execute it to create tables (Users, Transactions, Billers, BillPayments).
💻 How to Run the Project locally
1. Install Required Softwares
Python 3.x: Download Python
VS Code: Download VS Code
SQL Server Express: Download MS SQL
2. Install Python Libraries
Open your terminal/command prompt and run:
code
Bash
pip install streamlit pyodbc pandas plotly
3. Configure Connection
In app.py, find the DB_SERVER variable and replace it with your own server name (found in SSMS):
code
Python
DB_SERVER = r'YOUR_PC_NAME\SQLEXPRESS'
4. Run the Application
Navigate to the project folder and run:
code
Bash
streamlit run app.py
5. Stop the Application
To stop the local server, press Ctrl + C in the terminal.
🎓 About the Author
I am a BS FinTech student at FAST-NUCES, Chiniot-Faisalabad Campus. This project serves as my final submission for the Database Management Systems course, showcasing my ability to integrate financial business requirements with technical database solutions.
