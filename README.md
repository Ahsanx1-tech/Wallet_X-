💳 WalletX Pro: Digital Wallet Management System
![alt text](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)

![alt text](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)

![alt text](https://img.shields.io/badge/MS_SQL_Server-CC2927?logo=microsoft-sql-server&logoColor=white)

![alt text](https://img.shields.io/badge/FAST--NUCES-CFD_Campus-004184)
WalletX Pro is a full-stack financial dashboard developed as the Final Project for the Database Management Systems course (4th Semester). It simulates a modern mobile money environment, focusing on ACID-compliant transactions, relational data integrity, and real-time business intelligence.
📑 Table of Contents
Core Features
Tech Stack
Database Architecture
Installation & Setup
Usage Guide
About the Author
🚀 Core Features
User Onboarding: Dynamic customer registration with real-time validation and initial deposit handling.
P2P Transfers: Secure peer-to-peer money transfers using SQL Transaction logic (Commit/Rollback) to ensure data atomicity.
Utility Bill Payments: Integrated module to pay bills for various providers (e.g., LESCO, PTCL) with automatic balance deduction.
Business Intelligence (BI) Dashboard:
Real-time metrics tracking (Active Users, Total Liquidity, Transaction Volume).
Data visualization for revenue distribution by category using Plotly.
Admin Governance: Advanced search filters by name and balance, alongside secure account deletion protocols.
🛠 Tech Stack
Component	Technology
Frontend	Streamlit
Backend Logic	Python 3.x
Database	Microsoft SQL Server
Data Processing	Pandas
Visualization	Plotly Express
Connectivity	pyodbc
📂 Database Setup
Install SSMS: Ensure you have SQL Server Management Studio installed.
Create Database: Open SSMS and run:
code
SQL
CREATE DATABASE WalletX;
Import Schema: Open the WalletX_Database.sql file included in this repository and execute it. This script will:
Create tables: Users, Billers, Transactions, and BillPayments.
Seed the database with sample billers and account types.
💻 Installation & Setup
1. Software Prerequisites
Install the following if you haven't already:
Python 3.x
Visual Studio Code
SQL Server Express
2. Clone & Install Dependencies
Open your terminal and run:
code
Bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/Wallet_X-.git

# Navigate to the directory
cd Wallet_X-

# Install required libraries
pip install streamlit pyodbc pandas plotly
3. Configure Connection
Open app.py and update your Server Name found in SSMS:
code
Python
# app.py
DB_SERVER = r'YOUR_PC_NAME\SQLEXPRESS'
🏃 Usage Guide
Start the Application
Run the following command in your terminal:
code
Bash
streamlit run app.py
The application will automatically open in your default browser at http://localhost:8501.
Stop the Application
To shut down the local server, go back to your terminal and press:
Ctrl + C
🎓 About the Author
[Your Name Here]
BS FinTech | 4th Semester
FAST-NUCES (Chiniot-Faisalabad Campus)
This project was developed to demonstrate the intersection of Financial Technology and Database Management. It showcases the ability to translate business requirements into a functional, user-centric application while maintaining strict database standards.
📄 License
This project is for academic purposes. Please feel free to reach out for collaborations!
