# 📊 StockSight – Apache Superset Stock Market Analysis Dashboard

This project is a stock market visualization dashboard built with **Apache Superset** and connected to a **MySQL (or SQLite/SQL Server)** backend for querying historical stock data. It enables interactive analysis of selected stocks using visual tools like line charts, candlestick charts, correlation matrices, and more.

---

## 🛠️ Features

- 📈 Visualize trends in price, volume, and performance for 5 companies
- 🧠 Integrated with RNN-based predictive models (extension)
- ⚡ Real-time slicing and filtering on charts
- 🛠️ Powered by open-source Apache Superset and SQL database
- 🎥 [Demo Video](./Assests/Apache%20Superset%20Demo.mp4)

---

## 🚀 Setup Instructions

### 1. Clone the Project
```bash
git clone https://github.com/shubh4m-kumar/Stock-Market-Visualization-and-Forecasting-Dashboard-using-Apache-Superset-MySQL-and-RNN-

cd Stock-Market-Visualization-and-Forecasting-Dashboard-using-Apache-Superset-MySQL-and-RNN-
```

### 2. Create and Activate Virtual Environment
```bash
python -m venv "Stock-Market-Visualization-and-Forecasting-Dashboard-using-Apache-Superset-MySQL-and-RNN-
\.venv"
"Stock-Market-Visualization-and-Forecasting-Dashboard-using-Apache-Superset-MySQL-and-RNN-
\.venv\Scripts\activate"
```

### 3. Install Superset
```bash
pip install apache-superset
```

### 4. Set Environment Variables (PowerShell)
```powershell
$env:FLASK_APP = "superset"
$env:SUPERSET_CONFIG_PATH = "Stock-Market-Visualization-and-Forecasting-Dashboard-using-Apache-Superset-MySQL-and-RNN-
\superset_config.py"
```

### 5. Initialize Superset
```bash
superset db upgrade
superset fab create-admin  # Create admin user
superset init
```

### 6. Database Configuration

Edit `superset_config.py` or set one of the following:

#### For SQLite
```python
SQLALCHEMY_DATABASE_URI = 'sqlite:///D:\Qriocity\Apache Superset\stock_data.db'
```

#### For SQL Server
```python
SQLALCHEMY_DATABASE_URI = r'mssql+pyodbc://@localhost/master?driver=ODBC Driver 17 for SQL Server;Trusted_Connection=yes;'
```

### 7. Run Superset
```bash
superset run -p 8088 --with-threads --reload --debugger
```

Now visit `http://localhost:8088` in your browser and log in using the admin credentials you created.

---

## 🧠 About

This project was built as part of a data visualization + analytics stack for analyzing and predicting stock market behavior in a unified platform using **Apache Superset**, **SQL**, and optionally **RNN models** for future forecasting.

---

## 📬 Contact
📫 Reach out: shubhambpn1234@gmail.com
