# DVD Rental Database Analytics

## Overview

This project analyzes a PostgreSQL DVD rental database using Python and SQL. The goal of the project is to explore customer rental behavior, film inventory, return status, and business performance using a relational database workflow.

The project connects Python to a PostgreSQL database, runs SQL queries against the DVD rental schema, and presents results that could support business decision-making for a video rental company.

This project demonstrates practical skills in SQL, relational databases, Python database connectivity, and business analytics.

---

## Business Problem

A DVD rental business needs to understand how customers interact with its rental inventory. Important questions include:

- Which customers currently have unreturned films?
- Which films are rented most often?
- Which customers are the most active renters?
- How can rental data be used to identify operational issues?
- What insights can be drawn from customer, film, inventory, and rental tables?

By answering these questions, the business can better understand customer behavior, track inventory, and improve rental operations.

---

## Project Goals

The main goals of this project were to:

1. Connect a Python application to a PostgreSQL database.
2. Query a relational database using SQL.
3. Analyze rental, customer, film, and inventory data.
4. Identify meaningful business insights from the database.
5. Build a clean Python project structure suitable for submission and portfolio use.

---

## Tools and Technologies

- **Python**
- **PostgreSQL**
- **pgAdmin**
- **psycopg2**
- **SQL**
- **DVD Rental Sample Database**

---

## Dataset

This project uses the PostgreSQL DVD Rental sample database. The database contains information about:

- Customers
- Films
- Actors
- Categories
- Stores
- Staff
- Inventory
- Rentals
- Payments

The data is stored across multiple related tables, allowing for analysis using joins, filtering, grouping, and aggregation.

---

## Key Database Tables Used

Some of the main tables used in this project include:

| Table | Description |
|---|---|
| `customer` | Customer information |
| `rental` | Rental transaction records |
| `inventory` | Physical film copies available for rental |
| `film` | Film titles and metadata |
| `payment` | Payment records |
| `staff` | Staff members handling rentals |
| `store` | Store location information |

---

## Example Questions Answered

This project explores questions such as:

### 1. Which customers have unreturned films?

This query identifies customers with rentals where the `return_date` is missing. These records represent films that have not yet been returned.

### 2. Which films are rented most often?

This analysis joins the rental, inventory, and film tables to count how often each film has been rented.

### 3. Which customers have the most rentals?

This query ranks customers by total rental activity.

### 4. What films are currently checked out?

This query identifies inventory items that are associated with rentals that have not yet been returned.

### 5. What rental patterns can be identified from the database?

The project uses SQL queries to summarize activity and uncover operational insights.

---

## Project Structure

```text
dvd-rental-analytics/
│
├── README.md
├── main.py
├── requirements.txt
├── database.py
├── queries.py
├── analysis.py
└── screenshots/
