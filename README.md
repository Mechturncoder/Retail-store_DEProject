
# MySQL Integration with Python and Pandas

This project demonstrates how to integrate **Python**, **Pandas**, and **MySQL** to manage and analyze data. The workflow includes creating a database schema, interacting with MySQL using **SQLAlchemy**, and transferring data between a Pandas DataFrame and a MySQL database.

---

## Project Contents

1. **`orders.ipynb`**  
   A Jupyter Notebook that:
   - Establishes a connection with a MySQL database.
   - Demonstrates how to load data into a Pandas DataFrame.
   - Writes the DataFrame into a MySQL database table (`df_orders`).

2. **`sql_code.sql`**  
   A SQL script containing:
   - Schema definitions.
   - Table creation queries.
   - Other SQL operations relevant to the project.

---

## Prerequisites

1. **Python Libraries**:
   - `pandas`
   - `sqlalchemy`
   - `pymysql` or `mysqlclient` (for MySQL driver)

   Install them using pip:
   ```bash
   pip install pandas sqlalchemy pymysql
   ```

2. **MySQL Server**:
   - A MySQL instance must be running and accessible.
   - You need valid credentials (username, password, host, database name).

3. **Jupyter Notebook** (for `.ipynb` file):
   ```bash
   pip install notebook
   ```

---

## How to Run the Project

### Step 1: Set Up MySQL Database
1. Open the `sql_code.sql` file.
2. Execute the SQL commands in your MySQL Workbench or any SQL client to create the necessary database and tables.

### Step 2: Configure Python Script
1. Update the connection details in the script or notebook:
   ```python
   username = 'your_username'
   password = 'your_password'
   host = 'localhost'
   port = '3306'
   database = 'your_database'
   ```

2. Run the `orders.ipynb` notebook or Python script.

---

## Key Features

1. **SQLAlchemy Integration**:
   - Establishes robust and efficient connections with MySQL.

2. **Pandas `to_sql` Method**:
   - Transfers data seamlessly between Pandas DataFrames and MySQL tables.

3. **SQL File for Database Schema**:
   - Ensures easy replication of database structure.

---

## Notes

- Use **`if_exists='replace'`** with caution; it drops and recreates the table, erasing previous data.
