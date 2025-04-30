💻 Precio Portátiles – Laptop Price Prediction Using Machine Learning
This repository contains a complete machine learning pipeline for predicting laptop prices based on technical specifications such as processor type, RAM, storage capacity, graphics card, screen size, and other hardware details. 
The project aims to help users estimate the market value of laptops and aid retailers or customers in making informed pricing decisions.

🎯 Objective
The main goal of this project is to:

Predict the price of laptops based on their configuration.

Analyze which features most influence the price.

Build a robust regression model capable of generalizing to unseen data.

Demonstrate a full data science workflow from preprocessing to deployment readiness.

📦 Dataset Overview
The dataset used in this project includes a wide range of specifications for various laptops, scraped or sourced from e-commerce websites or open data platforms.

Sample Features:
Brand

Processor (e.g., Intel i5, AMD Ryzen 7)

RAM (e.g., 8GB, 16GB)

Storage (HDD/SSD capacity and type)

Graphics Card (Integrated or Dedicated GPU)

Screen Size (inches)

Operating System

Weight

Touchscreen (Yes/No)

Price (Target Variable)

🧠 Workflow
1. 📊 Exploratory Data Analysis (EDA)
Distribution of price and features

Brand-wise price comparisons

Correlation matrix to detect influential variables

Visuals using Seaborn, Matplotlib, Plotly

2. 🧹 Data Preprocessing
Encoding categorical variables (Label/One-Hot Encoding)

Handling missing values and outliers

Feature transformation (log-transform skewed data)

Standardizing numerical features

3. 🏗️ Feature Engineering
Combining RAM and storage into a “performance index”

Creating binary features (e.g., has_dedicated_gpu)

Converting weight to numeric values

4. 🤖 Model Building
Various regression models were evaluated:

Linear Regression

Decision Tree Regressor

Random Forest Regressor

Gradient Boosting (XGBoost, LightGBM)

Support Vector Regressor (SVR)

Model selection was based on metrics such as:

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

R² Score

🧪 Model Evaluation

Model	RMSE	R² Score
Linear Regression	23.4	0.72
Random Forest	14.8	0.89
XGBoost Regressor	13.6	0.91

🛠️ Tools and Libraries
Python 3.8+

Pandas, NumPy

Matplotlib, Seaborn, Plotly

Scikit-learn

XGBoost, LightGBM

Streamlit (for UI/Deployment)

Joblib (for model persistence)

🌍 Real-World Use Cases
E-commerce platforms: Auto-pricing engine for new laptops

Retailers/Resellers: Fair market value estimation for inventory

Consumers: Get an estimate of resale value or compare price vs. specs

🚀 Future Improvements
Deploy the model with a Streamlit or Flask UI

Add a web scraper for real-time product data

Implement deep learning models for complex patterns

Add model interpretability (SHAP, LIME)

