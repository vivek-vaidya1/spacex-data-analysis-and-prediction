# SpaceX Falcon 9 First Stage Landing Prediction

## Project Overview

This project was developed as part of the IBM Applied Data Science Capstone. The objective is to predict whether the Falcon 9 first stage will successfully land after launch. Since SpaceX reuses Falcon 9 boosters, successful landings significantly reduce launch costs. Predicting landing outcomes helps estimate launch costs and provides valuable insights for companies competing in the commercial space industry.

## Business Problem

SpaceX offers Falcon 9 launches at a significantly lower cost than traditional launch providers due to reusable rocket technology. Understanding the factors that influence successful booster landings can help estimate mission costs and support strategic decision-making.

## Project Workflow

### 1. Data Collection

* Collected launch data using the SpaceX REST API.
* Gathered mission details, payload information, launch sites, booster versions, and landing outcomes.
* Performed data cleaning and preprocessing.

### 2. Web Scraping

* Extracted Falcon 9 launch records from Wikipedia using BeautifulSoup.
* Parsed HTML tables and converted them into structured Pandas DataFrames.

### 3. Exploratory Data Analysis (EDA)

* Analyzed launch success rates across launch sites and booster versions.
* Identified trends using Pandas, Matplotlib, and Seaborn.
* Generated training labels for machine learning models.

### 4. SQL Analysis

* Loaded launch data into IBM Db2.
* Executed SQL queries to answer business and operational questions.
* Performed data aggregation and filtering for deeper insights.

### 5. Geospatial Analysis

* Used Folium to visualize launch locations.
* Mapped successful and failed launches.
* Analyzed geographical patterns affecting mission outcomes.

### 6. Interactive Dashboard

* Developed an interactive Plotly Dash dashboard.
* Implemented dropdown filters, range sliders, pie charts, and scatter plots.
* Enabled dynamic exploration of launch data.

### 7. Machine Learning

* Applied feature engineering and data preprocessing.
* Trained and evaluated multiple classification models:

  * Logistic Regression
  * Support Vector Machine (SVM)
  * K-Nearest Neighbors (KNN)
  * Decision Tree Classifier
* Performed hyperparameter tuning using GridSearchCV.

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| Decision Tree       | 94.44%   |
| SVM                 | 83.33%   |
| KNN                 | 83.33%   |
| Logistic Regression | 83.33%   |

**Best Model:** Decision Tree Classifier with 94.44% accuracy.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Dash
* BeautifulSoup
* SQL (IBM Db2)
* Scikit-learn
* Folium



## Key Skills Demonstrated

* Data Collection & API Integration
* Web Scraping
* Data Cleaning & Wrangling
* Exploratory Data Analysis
* SQL Querying
* Data Visualization
* Geospatial Analysis
* Machine Learning
* Hyperparameter Tuning
* Dashboard Development

## Conclusion

This project successfully predicts Falcon 9 first-stage landing outcomes using machine learning techniques. The Decision Tree model achieved the highest accuracy and demonstrated the strongest predictive performance. The project showcases an end-to-end data science workflow from data acquisition to deployment-ready visualization.
