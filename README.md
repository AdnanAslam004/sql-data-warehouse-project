SQL Data Warehouse Project

This project is a SQL data warehouse built using SQL Server and SQL Server Management Studio (SSMS).

I completed it to practise data warehousing, ETL processes, data cleaning, data quality checks, and dimensional modelling. The project combines data from CRM and ERP source systems and processes it through Bronze, Silver, and Gold layers.

Data Architecture



The project follows the Medallion Architecture:

Bronze Layer: Stores raw CRM and ERP data imported from CSV files.

Silver Layer: Cleans, standardizes, and transforms the raw data.

Gold Layer: Provides business-ready fact and dimension views for analysis.

Data Model



The Gold layer uses a star schema containing:

gold.fact_sales

gold.dim_customers

gold.dim_products

What I Did

Created the database and Bronze, Silver, and Gold schemas

Loaded CRM and ERP data from CSV files

Cleaned and standardized customer, product, location, and sales data

Handled duplicates, missing values, invalid dates, and inconsistent values

Built stored procedures for data loading and transformation

Created customer and product dimensions

Created the sales fact view

Performed data quality and referential-integrity checks

Designed the data architecture and star-schema diagrams

Tools Used

SQL Server

SQL Server Management Studio

T-SQL

CSV files

Draw.io

Git and GitHub

Repository Structure

data-warehouse-project/
│
├── datasets/                 # CRM and ERP source files
├── docs/                     # Architecture, data-flow, and data-model files
├── scripts/
│   ├── bronze/               # Raw-data loading scripts
│   ├── silver/               # Cleaning and transformation scripts
│   └── gold/                 # Fact and dimension views
├── tests/                    # Silver and Gold quality checks
├── README.md
├── LICENSE
└── .gitignore

How to Run the Project

Install SQL Server and SQL Server Management Studio.

Download or clone this repository.

Open the SQL scripts in SSMS.

Update the CSV file paths according to the location of the datasets on your computer.

Run the database initialization script.

Run the Bronze-layer scripts.

Run the Silver-layer scripts.

Run the Gold-layer scripts.

Run the scripts in the tests folder to verify data quality.

Warning: The database initialization script drops and recreates the DataWarehouse database if it already exists. Back up any important data before running it.

What I Learned

This project helped me understand how raw data moves through different warehouse layers before becoming ready for reporting and analysis. I also gained practical experience in ETL development, data cleaning, SQL views, stored procedures, data-quality testing, and star-schema modelling.

Credits

This project was completed for learning and portfolio purposes by following the SQL Data Warehouse Project by Data With Baraa. The original learning material provided the project structure, datasets, and guidance.

Author

Adnan AslamBachelor of Business Data Analytics student interested in SQL, data analytics, business intelligence, and data engineering.
