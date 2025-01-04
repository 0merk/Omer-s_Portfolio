# Omer-s_Portfolio
Analytics portfolio

# [Financial Econometrics and House Price Prediction Projects](https://github.com/0merk/Financial_Econometrics)

This repository showcases two major projects:  
1. Financial Econometric Modeling: Forecasting NVIDIA share prices and analyzing U.S. macroeconomic indicators.  
2. Machine Learning Models for House Price Prediction: Comparing Linear Regression, Random Forest, and Support Vector Regression (SVR).

---

## **Project 1: Financial Econometric Modeling**

### **1. Forecasting NVIDIA Share Prices**

#### Objective
Forecast NVIDIA's weekly share prices using econometric modeling techniques.

#### Methodology
- **Stationarity Tests:** Applied Augmented Dickey-Fuller (ADF) and KPSS tests to evaluate stationarity. Log differencing was used to transform the non-stationary series.
- **Seasonal Decomposition:** Decomposed the series into trend, seasonality, and noise using an additive model.
- **Model Selection:** Explored ARMA and ARIMA models, leveraging ACF and PACF plots for lag determination. Models were optimized based on AIC, BIC, and HQIC scores.
- **Findings:**
  - ARIMA (0,0,0) was the best-fit model, revealing that past values and residuals had no significant impact on future stock prices.
  - Suggested further analysis of external factors influencing stock price movements.

#### Tools Used
- Python: `Pandas`, `Statsmodels`, `Matplotlib`

---

### **2. Analyzing U.S. Macroeconomic Indicators**

#### Objective
Analyze and forecast the relationship between U.S. GDP Growth Rate and Unemployment Rate.

#### Methodology
- **Stationarity Tests:** Conducted ADF tests to confirm stationarity after differencing.
- **Causality Analysis:** Used Granger Causality tests to establish bidirectional causality between unemployment and GDP growth.
- **Modeling Approach:**
  - Developed a Vector Autoregressive (VAR) model with lag selection based on informational criteria.
  - Conducted impulse response analysis to evaluate dynamic relationships between variables.
  - Generated 20-step forecasts for both unemployment and GDP growth.
- **Findings:**
  - Strong interdependence observed between the two variables.
  - Recommended the inclusion of additional external economic factors for enhanced forecasting accuracy.

#### Tools Used
- Python: `Statsmodels`, `Matplotlib`, `Pandas`

---

# [Mindset Institute Büyük veri ve İş Analitiği Uzmanlığı Sertifika Programı](https://github.com/0merk/mindset_big_data)

## **Project : House Price Prediction**

#### Objective
Develop a system to predict house prices using three regression models: Linear Regression, Random Forest Regression, and Support Vector Regression (SVR).

#### Methodology

##### Data Loading and Exploration
- **Data Exploration:**
  - Loaded the `house.csv` dataset into a pandas DataFrame (`df`).
  - Performed basic data analysis using `df.head()`, `df.tail()`, `df.shape`, `df.info()`, and `df.describe()`.
- **Visualization:**
  - Plotted correlations using a heatmap (`seaborn.heatmap`).
  - Detected outliers with box plots for each feature.
- **Outlier Removal:** 
  - Applied the IQR method to clean the `price` column.

##### Linear Regression Model
- **Data Preparation:**
  - Separated features (`X`) and target variable (`y`).
  - Scaled features using `StandardScaler`.
  - Split the dataset into training and testing sets with `train_test_split`.
- **Model Training:** Trained a Linear Regression model.
- **Model Evaluation:**
  - Calculated Mean Squared Error (MSE) and R-squared (R²).
  - Visualized predictions vs. actual values using a scatter plot.
  - Analyzed residuals and calculated adjusted R-squared.

##### Random Forest Regression Model
- **Model Training:** Built a Random Forest Regression model.  
- **Model Evaluation:**  
  - Computed R-squared error.
  - Plotted actual vs. predicted prices with a line plot.

##### Support Vector Regression (SVR) Model
- **Data Preparation:** Similar to the Linear Regression process.
- **Model Training:** Trained an SVR model with a linear kernel.
- **Model Evaluation:**  
  - Plotted actual vs. predicted values.  
  - Analyzed residuals.  
  - Displayed feature coefficients.

---

### **Findings**
- Identified key preprocessing steps like outlier removal and feature scaling as critical for model performance.  
- Demonstrated the strengths and weaknesses of each regression model:
  - **Linear Regression:** Simple and interpretable but may lack flexibility.  
  - **Random Forest:** Non-linear and robust, providing strong performance.  
  - **SVR:** Effective for small datasets with linear relationships but computationally intensive.

#### Tools Used
- Python: `Pandas`, `Matplotlib`, `Seaborn`, `Scikit-learn`

---

Feel free to explore the code and analysis files for these projects in the repository. Contributions and suggestions are welcome!
