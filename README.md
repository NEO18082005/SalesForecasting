# 📈 End-to-End Sales Forecasting & Demand Intelligence System

Welcome to my **End-to-End Sales Forecasting & Demand Intelligence System** repository! This project was developed during Week 3 and Week 4 of my data science internship. It is a multi-layered, real-world industry project focusing on time-series analysis, machine learning forecasting, anomaly detection, and product segmentation.

## 🎯 Project Overview
Every retail company relies on accurate sales predictions to manage inventory efficiently. Overstock wastes capital, while understock loses customers. This project tackles that exact problem by building an AI-driven system that:
1. **Predicts future product demand** across different categories and regions.
2. **Detects unusual sales spikes or drops** (anomalies) using advanced statistical and machine learning methods.
3. **Segments products** by demand behavior to recommend specific stocking strategies.
4. **Visualizes the insights** via a fully interactive, deployed web dashboard.

## 🗂️ Repository Structure (Submission Folder)
As per the project requirements, this repository contains all the necessary files for final submission:

- `analysis.ipynb` — Complete Jupyter Notebook containing all 8 tasks, with markdown explanations, EDA, modeling, and evaluation.
- `train.csv` — The primary Superstore sales dataset containing 4 years of daily sales data.
- `vgsales.csv` — The supplementary dataset used to perform multi-source multivariate anomaly detection.
- `app.py` — The Python script powering the interactive Streamlit dashboard.
- `requirements.txt` — All Python dependencies required to run the notebook and deploy the dashboard.
- `summary.pdf` — The 2-page Executive Business Report summarizing findings and recommendations for the Head of Supply Chain and CFO.
- `charts/` — A directory containing all the exported chart images (.png) generated during the analysis.

## 🛠️ Technologies & Models Used
- **Languages & Libraries:** Python 3.x, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly
- **Time Series & Forecasting:** Statsmodels (SARIMA), Facebook Prophet, XGBoost (Supervised ML formulation)
- **Anomaly Detection:** Isolation Forest (Multivariate), Z-Score (Shifted Rolling Window)
- **Clustering:** K-Means, PCA (Principal Component Analysis)
- **Deployment:** Streamlit Community Cloud

## 🚀 Live Dashboard
Check out the fully functional, interactive Streamlit dashboard here:
👉 **[Live Streamlit App](https://demand-intelligence-system-1808.streamlit.app/)**

## 📊 Key Technical Highlights
- **Forecasting:** Evaluated SARIMA, Prophet, and XGBoost. **Prophet** was selected as the best production model due to its robust handling of massive yearly holiday seasonality, achieving the lowest Mean Absolute Percentage Error (MAPE).
- **Anomaly Detection:** Implemented a robust multi-source approach using both *Isolation Forest* (global distribution) and shifted *Z-Scores* (local momentum) to flag massive Q4 spikes and unexpected mid-year supply chain drops.
- **Product Segmentation:** Used K-Means clustering and the Elbow Method to segment sub-categories into 4 distinct demand groups (e.g., *High Value Volatile*, *Steady Bulk*) to recommend targeted inventory policies like Just-In-Time (JIT) ordering.

---
*This repository serves as the final evaluation submission for the Week 3 & 4 Internship Project.*
