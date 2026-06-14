# 💳 WalletX Pro: Digital Wallet Management System

![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)
![MS SQL Server](https://img.shields.io/badge/MS_SQL_Server-CC2927?logo=microsoft-sql-server&logoColor=white)
![FAST-NUCES CFD Campus](https://img.shields.io/badge/FAST--NUCES-CFD_Campus-004184)

**WalletX Pro** is a full-stack financial dashboard developed as the **Final Project for the Database Management Systems course (4th Semester)**. It simulates a modern mobile money environment, focusing on ACID-compliant transactions, relational data integrity, and real-time business intelligence.

---

## 📑 Table of Contents
* [Core Features](#-core-features)
* [Tech Stack](#-tech-stack)
* [Database Setup](#-database-setup)
* [Installation & Setup](#-installation--setup)
* [Usage Guide](#-usage-guide)
* [About the Author](#-about-the-author)

---

## 🚀 Core Features

- **User Onboarding:** Dynamic customer registration with real-time validation and initial deposit handling.
- **P2P Transfers:** Secure peer-to-peer money transfers using **SQL Transaction logic** (Commit/Rollback) to ensure data atomicity.
- **Utility Bill Payments:** Integrated module to pay bills for various providers (e.g., LESCO, PTCL) with automatic balance deduction.
- **Business Intelligence (BI) Dashboard:** 
    - Real-time metrics tracking (Active Users, Total Liquidity, Transaction Volume).
    - Data visualization for revenue distribution by category using Plotly.
- **Admin Governance:** Advanced search filters by name and balance, alongside secure account deletion protocols.

---

## 🛠 Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | [Streamlit](https://streamlit.io/) |
| **Backend Logic** | [Python 3.x](https://www.python.org/) |
| **Database** | [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server/) |
| **Data Processing** | [Pandas](https://pandas.pydata.org/) |
| **Visualization** | [Plotly Express](https://plotly.com/python/) |
| **Connectivity** | [pyodbc](https://github.com/mkleehammer/pyodbc) |

---

## 📂 Database Setup

1.  **Install SSMS:** Ensure you have [SQL Server Management Studio](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms) installed.
2.  **Create Database:** Open SSMS and run:
    ```sql
    CREATE DATABASE WalletX;
    ```
3.  **Import Schema:** Open the `.sql` file included in this repository and execute it. This script will:
    - Create tables: `Users`, `Billers`, `Transactions`, and `BillPayments`.
    - Seed the database with sample billers and account types.

---

## 💻 Installation & Setup

### 1. Software Prerequisites
*   [Python 3.x](https://www.python.org/downloads/)
*   [Visual Studio Code](https://code.visualstudio.com/)
*   [SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

### 2. Install Dependencies
Open your terminal and run:
```bash
pip install streamlit pyodbc pandas plotly

3. Configure Connection
Open app.py and update your Server Name found in SSMS:

DB_SERVER = r'YOUR_PC_NAME\SQLEXPRESS'

🏃 Usage Guide
Start the Application
Run the following command in your terminal:

streamlit run app.py

Stop the Application
Press Ctrl + C in the terminal to shut down the server.
