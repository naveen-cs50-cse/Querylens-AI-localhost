# NeuralBI-AI-Dashboard
# Conversational AI Business Intelligence Dashboard

![Node.js](https://img.shields.io/badge/Backend-Node.js-green)
![JavaScript](https://img.shields.io/badge/Language-JavaScript-yellow)
![Chart.js](https://img.shields.io/badge/Visualization-Chart.js-blue)
![SQLite](https://img.shields.io/badge/Database-SQLite-lightgrey)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

An **AI-powered analytics dashboard** that converts natural language questions into SQL queries and automatically generates meaningful data visualizations.

Instead of writing SQL queries or manually creating charts, users can simply ask questions in plain English and instantly receive insights through dynamically generated graphs.

---

# Demo

Example user question:

```id="dcj2vt"
Show the distribution of shopping preferences
```

Generated SQL query:

```sql id="c9q0s7"
SELECT shopping_preference, COUNT(*) AS total_users
FROM customer_behavior
GROUP BY shopping_preference;
```

Result:

Automatically generated visualization displaying the distribution of users by shopping preference.

---

# Features

### Natural Language Querying

Users can ask questions in English and the system automatically converts them into SQL queries.

### Automatic Data Visualization

The system analyzes the query results and generates the most suitable chart automatically.

Supported charts:

* Bar charts
* Line charts
* Pie charts
* Scatter plots

### Smart Chart Interpreter

The visualization engine intelligently:

* detects categorical and numeric columns
* generates proper chart titles
* creates readable axis labels
* formats column names
* limits large datasets for readability

### Conversational Data Exploration

Users can explore datasets interactively without needing SQL or data analysis skills.

---

# System Architecture

```id="zbuhyq"
User Question (Natural Language)
                ↓
        AI Query Interpreter
                ↓
            SQL Query
                ↓
        SQLite Database
                ↓
          Query Results
                ↓
     Smart Chart Interpreter
                ↓
      Chart.js Visualization
```

---

# Tech Stack

## Frontend

* HTML
* CSS
* JavaScript
* Chart.js

## Backend

* Node.js
* Express.js

## Database

* SQLite

## AI Layer

* Natural Language → SQL generation

---

# Example Questions

Users can ask questions such as:

* What is the distribution of shopping preferences?
* Show monthly sales trends
* Which product category has the highest revenue?
* Compare online and store purchases
* Show average income by customer group

The system automatically converts these questions into SQL queries and generates charts.

---

# Installation

Clone the repository:

```id="t1zly6"
git clone https://github.com/yourusername/ai-bi-dashboard.git
cd ai-bi-dashboard
```

Install dependencies:

```id="tvz9s6"
npm install
```

Start the server:

```id="owr8e4"
node server.js
```

Open in browser:

```id="83g5z1"
http://localhost:2000
```

---

# Project Goals

The goal of this project is to simplify data analysis by enabling conversational interaction with databases.

Instead of writing SQL queries or building dashboards manually, users can simply ask questions and instantly receive insights through automatically generated visualizations.

---

# Future Improvements

* AI generated dashboards (multiple charts)
* Interactive filtering
* continuous chat

---

# License

This project is licensed under the MIT License.
