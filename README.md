# Personal-Finance-Dashboard

# Introduction

This project represents my effort to apply data analytics and software development skills to solve a real-life problem — understanding and managing personal finances effectively.

I designed and developed a MySQL database named spend_save to systematically track and analyze financial transactions such as purchases, deposits, withdrawals, and credit card payments. My goal was not only to store financial data but also to convert raw banking data into meaningful insights.

To achieve this, I collected transaction data from banking platforms in CSV format, transformed and cleaned the data using Python libraries such as Pandas and NumPy, and loaded it into the database using SQLAlchemy. Finally, I built SQL views and an interactive Power BI dashboard to visualize spending patterns and financial trends.

This project reflects my interest in combining data engineering, analytics, and visualization to create data-driven solutions.

# Technologies and Skills
**Technologies Used**

SQL (MySQL)

MySQL Workbench

Python (Pandas, NumPy, SQLAlchemy)

Power BI

DAX

**Skills Demonstrated**

Database design and data modeling

ETL (Extract, Transform, Load) pipeline development

Data cleaning and transformation

Financial data analysis

Data visualization and dashboard development

Automation using Python

# Inspiration

I have always been curious about how daily spending impacts long-term financial stability. While I had a general idea of my expenses, I wanted a structured and analytical way to monitor them.

My main motivation behind this project was to:

Gain complete visibility into my spending habits

Identify high-expense categories

Track financial patterns across different months

Improve personal financial decision-making

Strengthen my practical data engineering and analytics skills

This project allowed me to learn by working on real-world data while solving a problem that directly affects everyday life.

# Identifying Requirements

Before building the system, I focused on defining clear requirements. My objective was to design a system capable of tracking every transaction occurring in savings accounts, checking accounts, and credit cards.

To achieve this, I needed to capture:

Transaction amount

Transaction date

Transaction category

Transaction type (purchase, deposit, payment, etc.)

Account details

This required extracting transaction-level data from banking sources and ensuring the data was structured and reliable for analysis.

# ER Diagram and Data Modeling

To efficiently store and analyze the financial data, I designed a dimensional data model consisting of:

Four dimension tables

account

transaction_type

category

date

One fact table

transaction_facts

The dimension tables provide descriptive information about each transaction, while the fact table stores the measurable financial transaction data.

I also implemented constraints to ensure data integrity. For example, transaction categories are only assigned to applicable transaction types such as debit or credit purchases.

This design helped me understand real-world data warehouse modeling concepts.

# Database Creation

The database was created using MySQL Workbench’s forward engineering feature. I implemented table relationships, constraints, and validation rules to ensure accurate and consistent data storage.

This phase helped me strengthen my understanding of relational database design and schema implementation.

# Loading Data into Dimension Tables

Dimension data was loaded using structured CSV files. These files contained predefined values such as account types, transaction categories, and date references.

This step ensured standardization and consistency across the entire database.

# Transaction Processing and Loading into Fact Table

Transaction data was collected from multiple banking accounts including savings accounts, checking accounts, and credit cards. The data was downloaded manually from banking portals as CSV files.

I processed this data using Python inside Jupyter Notebook by:

Cleaning inconsistent or missing values

Standardizing transaction descriptions

Formatting dates and numerical fields

Creating reusable automation functions

These custom Python functions reduced manual work and improved processing efficiency. For transactions that could not be processed automatically, I manually validated and corrected them.

This phase significantly improved my ETL development and data preprocessing skills.

# SQL Analysis and Database Views Creation

After loading the data into the database, I focused on extracting meaningful financial insights using SQL queries.

I developed multiple database views to analyze:

Monthly spending patterns

Category-wise expense distribution

Account balance trends

Saving behavior over time

Creating database views allowed quick and reusable access to analytical results and improved dashboard integration.

# Power BI Dashboard

To make the analysis more interactive and user-friendly, I developed a Power BI dashboard connected directly to the database.

The dashboard includes:

Monthly expense trend analysis

Category-wise spending visualization

Income vs expense comparison

Account balance tracking

Spending behavior insights

Through the dashboard, I discovered that a large portion of expenses was spent on non-essential categories, especially food and dining. I also identified seasonal spending trends where expenses increased during certain months.

# Project Outcome and Learning Experience

This project became a strong practical learning experience where I applied multiple technical concepts in one complete workflow. It helped me understand how raw data can be converted into valuable insights using structured databases, automation, and visualization tools.

Beyond technical skills, this project improved my analytical thinking and strengthened my understanding of financial data behavior.

Overall, this system acts as a personal financial monitoring tool while demonstrating my ability to build end-to-end data analytics solutions.
