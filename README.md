# 🍽️ SmartMeal: Food Demand Prediction & Waste Reduction Using PySpark

SmartMeal is a Big Data and Machine Learning-based food demand prediction platform designed to help canteens and food service providers make data-driven meal preparation decisions and reduce food waste.

The project uses **Apache PySpark** for large-scale data processing and **Random Forest Regression** to predict daily food demand based on historical consumption patterns, menu categories, weather conditions, holidays, promotions, and previous leftovers.

An interactive **Streamlit dashboard** presents demand forecasts, food preparation insights, leftover analysis, and model performance through visualizations and analytical reports.

## 🎯 Project Objectives

- Predict daily food demand using historical consumption data.
- Minimize food wastage through accurate demand forecasting.
- Optimize meal preparation based on predicted demand.
- Analyze consumption patterns across different menu categories.
- Apply Big Data processing techniques using Apache PySpark.
- Provide actionable insights through an interactive analytics dashboard.

## 🚀 Key Features

- **Data Generation:** Generates a synthetic food demand dataset containing 4,000 records representing canteen demand patterns from 2023 to 2025.
- **Data Cleaning:** Handles missing values, duplicate records, invalid entries, and categorical data using PySpark.
- **Feature Engineering:** Extracts date-based features and encodes menu categories, weekdays, and weekends.
- **Demand Prediction:** Implements Random Forest Regression using PySpark MLlib.
- **Model Evaluation:** Evaluates predictions using RMSE, MAE, and R² Score.
- **Feature Importance:** Identifies the factors that influence food demand.
- **Interactive Dashboard:** Visualizes actual demand, predicted demand, meals prepared, leftover quantities, and estimated surplus.
- **Dynamic Filtering:** Supports analysis by date range and menu category.

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Big Data Processing | Apache Spark, PySpark |
| Machine Learning | PySpark MLlib, Random Forest Regression |
| Data Analysis | Pandas, NumPy |
| Visualization | Plotly |
| Dashboard | Streamlit |
| Data Storage | CSV |

## 📊 Machine Learning Approach

**Algorithm:** Random Forest Regression

The model predicts the number of meals required using 16 input features, including:

- Year, month, day, and day of the week
- Temperature and holiday information
- Promotions and previous leftovers
- Menu category
- Weekday and weekend indicators

**Dataset Split:**
- Training Data: 2023–2024
- Testing Data: 2025

**Evaluation Metrics:**
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- R² Score

The model's feature importance analysis helps identify the variables that contribute most to food demand predictions.

## 🔄 Project Workflow

1. Generate the food demand dataset.
2. Perform data cleaning and preprocessing.
3. Apply feature engineering using PySpark.
4. Train the Random Forest Regression model.
5. Evaluate model performance.
6. Generate demand predictions and feature importance results.
7. Display analytical insights through the Streamlit dashboard.

## 📁 Project Structure

```text
SmartMeal/
│
├── generate_dataset.py
├── 01_data_cleaning.py
├── 02_feature_engineering.py
├── 03_model_training.py
├── app.py
│
├── food_demand.csv
├── cleaned_food_demand.csv
├── featured_food_demand.csv
├── model_predictions.csv
├── feature_importance.csv
│
└── README.md
```

## ⚙️ Installation and Setup

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/SmartMeal.git
cd SmartMeal
```

**2. Create a virtual environment**

```bash
python -m venv .venv
```

**3. Activate the environment**

Windows:

```bash
.venv\Scripts\activate
```

**4. Install dependencies**

```bash
pip install pyspark pandas numpy streamlit plotly
```

**5. Execute the project pipeline**

Run the following scripts in sequence:

```bash
python generate_dataset.py
python 01_data_cleaning.py
python 02_feature_engineering.py
python 03_model_training.py
```

**6. Launch the dashboard**

```bash
streamlit run app.py
```

## 📈 Expected Outcomes

SmartMeal provides a data-driven approach to food demand forecasting by combining distributed data processing, machine learning, and interactive visualization.

The platform helps users:
- Understand historical food consumption patterns.
- Estimate future meal requirements.
- Identify potential food surpluses.
- Analyze actual leftovers and unfulfilled demand.
- Make informed food preparation decisions.

## 📚 Dataset Information

The project uses a **synthetically generated dataset of 4,000 records** created using Python because real-world canteen consumption records were not available.

The dataset simulates realistic food demand patterns across different dates, menu categories, weather conditions, holidays, promotions, and leftover quantities.

It is designed for academic experimentation and demonstration of Big Data processing and predictive analytics.

## 👨‍💻 Author

**Gampala Vijay Kumar**

B.Tech Computer Science and Engineering

Lovely Professional University

GitHub: https://github.com/Vijay0567

---

*SmartMeal demonstrates the practical application of Big Data Analytics and Machine Learning to address food demand forecasting and food waste management challenges.*
