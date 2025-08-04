# 🛒 E-commerce Sales Analytics Platform

A comprehensive, end-to-end analytics platform for the **e-commerce domain**, built on Python, SQL Server, and Azure. This project provides a robust foundation for modern sales analytics, integrating data extraction, transformation, visualization, and machine learning.

> 🚀 **Mission:** To deliver a production-grade, data-driven e-commerce platform that accelerates insights from raw data to actionable business intelligence while ensuring scalability and accuracy.

![Tech Stack Banner](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) ![Tech Stack Banner](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white) ![Tech Stack Banner](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white) ![Tech Stack Banner](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![Tech Stack Banner](https://img.shields.io/badge/Matplotlib-1363DF?style=for-the-badge&logo=matplotlib&logoColor=white) ![Tech Stack Banner](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![Tech Stack Banner](https://img.shields.io/badge/MLflow-009688?style=for-the-badge&logo=mlflow&logoColor=white)

---

## 📌 Key Features

*   **End-to-End Data Lifecycle:** Fully implemented data flow from database connection to interactive visualizations and predictive analytics.
*   **Data Integration & Exploration:** Connects to a SQL Server database, retrieves sales data, and performs comprehensive data analysis.
*   **Interactive Visualizations:** Generates insightful charts and graphs for customer demographics, product sales, and order trends.
*   **Machine Learning Forecasting:** Implements a Random Forest model for sales forecasting using MLflow for experiment tracking.
*   **Automated Reporting:** Includes pre-built Python scripts for data analysis and visualization.
*   **Scalable Architecture:** Designed for easy integration with cloud platforms like Azure for future scaling.

---

## 1.📁 Repository Structure

```plaintext
ecommerce-sales-analytics/
│
├── 📂 data/             # Sample e-commerce datasets (CSV, Excel)
├── 📂 notebooks/         # Jupyter Notebooks for data analysis and visualization
├── 📂 scripts/           # Python scripts for ETL, ML, and reporting
├── 📂 models/            # Trained ML models (MLflow format)
├── 📂 reports/           # Generated reports and visualizations
└── 📂 docs/              # Documentation and project notes
```

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

## 3. Configure Database Connection

```bash
server = ''
database = 'Ecommerce_Sales'
username = 'sa'
password = ''
```

## 4. Run Data Analysis
Execute the Jupyter Notebook or Python script to perform data analysis:

```bash
python analysis_script.py
```

## 5. 📊 Data Visualization Previews
The platform includes several pre-configured visualizations for immediate insights.

```plaintext
👤 Customer Age Distribution
🛍️ Product Types Distribution
📅 Daily Order Trends
```

6. 📦 Machine Learning Forecasting
The platform includes a sales forecasting model using Random Forest:

```python
# Sales forecasting with MLflow
from sklearn.ensemble import RandomForestRegressor
from sklearn.model_selection import train_test_split
import mlflow
from sklearn.metrics import mean_absolute_error

# Train model
model = RandomForestRegressor(n_estimators=100, max_depth=5, random_state=42)
model.fit(X_train, y_train)

y_pred = model.predict(X_test)
mae = mean_absolute_error(y_test, y_pred)

# Log metrics with MLflow
mlflow.log_metric("mae", mae)
mlflow.sklearn.log_model(model, "Sales_Forecasting_Model")
print(f"Sales Forecasting Model MAE: {mae}")
```

7. 📅 Project Roadmap
The platform includes a sales forecasting model using Random Forest:

```plaintext
Key milestones include:

Initial data extraction and connection
Comprehensive data analysis and visualization
Implementation of machine learning forecasting
Integration with Power BI for business reporting
Deployment to Azure cloud platform
```

✅ **Tips:**
```plaintext
- Replace `YOUR_USERNAME` with your actual GitHub username.
- Replace placeholder image URLs with actual image paths if you upload screenshots to your repo (e.g., `![Customer Age Distribution](images/age_distribution.png)`).
- Add a `requirements.txt` file to your project with:
```
