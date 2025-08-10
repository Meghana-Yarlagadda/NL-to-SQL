
---

# 📊 CRM Database for Second-Hand Car Market with AI-Powered Querying

## 📌 Overview

This project demonstrates the creation, management, and analysis of a **CRM database** for a **second-hand car market**. It combines **SQL**, **Python**, and **Natural Language Processing (NLP)** to allow both technical and non-technical users to extract valuable business insights.

Key features include:

* **Realistic dataset generation** using Python’s `Faker` library
* **SQL Server** database integration with **SQLAlchemy** & **PyODBC**
* **Complex SQL queries** for actionable insights
* **AI-powered query translation** using OpenAI’s `GPT-3.5-turbo`
* **Natural language responses** for query results

---

## 🗂️ Dataset

Data is generated for:

* **Customers** – personal details, location, contact info
* **Cars** – make, model, price, year of manufacture
* **Sales** – agent details, transaction records

The dataset is stored in a **SQL Server database** and is designed for scalability and analytical purposes.

---

## 🛠️ Tech Stack

* **Python** (Data generation, NLP, automation)
* **SQL Server** (Relational database management)
* **SQLAlchemy** & **PyODBC** (Database connection & queries)
* **Faker** (Realistic test data generation)
* **OpenAI GPT-3.5-turbo** (Natural language to SQL translation)

---

## 🚀 Features

* **Automated Data Generation** – Populate database with realistic CRM data
* **Advanced SQL Queries** –

  * Most expensive car
  * Sales revenue by city
  * Top-performing sales agents
* **AI-Powered Querying** – Convert natural language to SQL queries
* **Natural Language Output** – SQL results converted into human-readable responses

---

## 📊 Example Queries

**Natural Language:** "Which city generated the highest sales revenue?"
**Generated SQL:**

```sql
SELECT TOP 1 City, SUM(SaleAmount) as TotalRevenue  
FROM Sales  
GROUP BY City  
ORDER BY TotalRevenue DESC;
```

**Natural Language Response:** "The city with the highest sales revenue is **Hyderabad** with ₹1,25,000 in total sales."

---

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/crm-ai-sql.git
cd crm-ai-sql
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Configure **SQL Server** connection in `config.py`
4. Set your **OpenAI API Key** as an environment variable:

```bash
export OPENAI_API_KEY="your_api_key"
```

5. Run the script:

```bash
python main.py
```

---

## 📈 Results

* **Improved data accessibility** for non-technical users
* **Streamlined database queries** via AI-powered automation
* **Enhanced decision-making** through instant insights

---

## 🙏 Acknowledgements

* [Faker](https://faker.readthedocs.io/) – Data generation
* [OpenAI](https://openai.com/) – GPT-3.5-turbo API
* [SQLAlchemy](https://www.sqlalchemy.org/) – Database ORM
* [PyODBC](https://github.com/mkleehammer/pyodbc) – SQL Server connectivity

---

