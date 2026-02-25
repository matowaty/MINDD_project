# Data Science & Predictive Modeling Portfolio

This repository showcases two comprehensive data science projects focusing on **Classification Modeling** and **Time-Series Forecasting**. Developed as a collaborative university project, both implementations follow the industry-standard **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology to solve real-world business problems.

### 👥 Team Members
* Mateusz Nowak
* Julia Kardasz
* Emilia Pawlowska

---

## 🏦 Project 1: Bank Telemarketing Campaign Prediction
**File:** `project.ipynb`

**Goal:** Build a data-driven model to predict the success of telemarketing calls for long-term bank deposits. By targeting only the most promising clients, banks can drastically reduce operational costs and increase marketing efficiency. 

**Dataset:** Historical customer, campaign, and macroeconomic data (2008–2013, during the Global Financial Crisis).

### 🛠️ Tech Stack & Methods
* **Languages & Libraries:** Python, Pandas, NumPy, Scikit-Learn, Imbalanced-learn, Matplotlib, Seaborn
* **Algorithms Tested:** Gradient Boosting, Random Forest, Decision Trees, SVM, Logistic Regression, KNN, Naive Bayes, Neural Networks.
* **Handling Imbalanced Data:** SMOTETomek, SMOTEENN.

### 🚀 Key Takeaways & Results
* **Business-Driven Metrics:** We recognized early on that standard *Accuracy* would be highly misleading due to class imbalance. We optimized for **AUC-PR and Precision**, directly aligning technical performance with the business goal of cost-effective marketing.
* **The Power of Boosting:** Advanced Gradient Boosting algorithms proved highly effective for this structured tabular data, significantly outperforming both simpler statistical models and more complex Neural Networks.

---

## ⚡ Project 2: Electricity Price Forecasting
**File:** `project2.ipynb`

**Goal:** Develop and compare statistical, machine learning, and deep learning models to accurately forecast hourly electricity prices one-step ahead and 24-steps (one day) ahead for grid operators and energy traders. 

**Dataset:** 4 years of hourly electricity prices, energy generation, and weather data (2015–2018).

### 🛠️ Tech Stack & Methods
* **Languages & Libraries:** Python, Pandas, Scikit-Learn, Statsmodels, XGBoost, LightGBM
* **Algorithms Tested:** SARIMAX, XGBoost, LightGBM, Support Vector Regression (SVR), Random Forest, Bagging & Gradient Boosting Regressors, Seasonal Naïve (Baseline).
* **Evaluation Metrics:** MAE, RMSE, MAPE.

### 🚀 Key Takeaways & Results
* **Features Matter:** We found that exogenous variables (weather, wind generation) physically drive the market. Baseline models failed because electricity prices aren't just a function of history—a model without weather forecasts will always fail during sudden storms.
* **Forecasting Strategy:** For real-world grid planning, a **Recursive Strategy** (predicting one hour, and using that prediction to predict the next) proved vastly superior to trying to output an entire 24-hour vector all at once. 

---

## 🎯 Skills Highlighted
* **End-to-End ML Pipeline:** Full implementation of CRISP-DM—from data collection and EDA to feature engineering and hyperparameter tuning.
* **Time-Series Analysis:** Handling seasonality, trends, and exogenous regressors in complex temporal data.
* **Advanced Data Processing:** Robust scaling, power transformations, and handling severely imbalanced datasets.
* **Business Acumen:** Translating abstract machine learning metrics into tangible business value and strategic recommendations.
