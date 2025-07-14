🔌 Power Consumption Forecasting - Wellington, NZ

Forecasting daily power consumption in Zone 1 of Wellington, New Zealand using machine learning techniques and environmental data.

⸻

📘 Project Overview

This project aims to build a predictive model to estimate energy consumption using meteorological and environmental variables. The goal is to assist power utility companies in resource planning and energy management.

⸻

📂 Dataset Description
	•	Records: 52,583
	•	Target: Power Consumption in A Zone (in KWR)
	•	Features:
	•	Temperature
	•	Humidity
	•	Wind Speed
	•	General Diffuse Flows
	•	Diffuse Flows
	•	Air Quality Index
	•	Cloudiness (binary)

⸻

🧹 Data Preprocessing
	•	Cleaned and renamed columns
	•	Converted object to numeric (Temperature, Humidity)
	•	Handled missing values using median imputation
	•	Removed outliers using IQR capping
	•	Feature engineering: Temp × Humidity interaction

⸻

📊 Exploratory Data Analysis
	•	Correlation matrix and heatmaps
	•	Distribution plots and boxplots
	•	Residual and error analysis
	•	Identified Temperature and Solar Radiation as key drivers

⸻

🤖 Models Implemented
	1.	Linear Regression
	2.	Random Forest Regressor (Best Performance)
	3.	XGBoost Regressor

Evaluation Metrics:

Model	R² Score	RMSE	MAE
Linear Regression	0.33	6563	5278
Random Forest	0.66	4702	3260
XGBoost	0.54	5472	4138


⸻

🛠️ Hyperparameter Tuning
	•	Used RandomizedSearchCV with 10-fold Cross Validation
	•	Best Parameters:
	•	n_estimators=200
	•	max_depth=40
	•	max_features=‘log2’

⸻

📈 Visual Diagnostics
	•	Actual vs Predicted scatter plot
	•	Residual plot
	•	Error histogram

⸻

💡 Business Insights
	•	Higher temperatures and radiation significantly increase energy demand
	•	Cloudy days = slightly reduced power usage
	•	Model can assist in:
	•	Peak load forecasting
	•	Dynamic grid optimization

⸻

✅ Tools Used
	•	Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib)
	•	Jupyter Notebook
	•	RandomizedSearchCV
	•	XGBoost

⸻

📃 License

This project is for educational and demonstration purposes only.
