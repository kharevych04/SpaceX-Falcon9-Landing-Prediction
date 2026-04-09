# SpaceX Falcon 9 Landing Prediction

**Capstone Project: IBM Data Science Professional Certificate**

## Project Overview

The goal of this project is to predict whether the SpaceX Falcon 9 first stage will land successfully. SpaceX significantly reduces the cost of space launches by reusing the first stage of their rockets. By predicting the probability of a successful landing, we can estimate the cost of a launch and determine if competing companies can effectively bid against SpaceX.

## Key Findings

* Best Performing Model: After tuning hyperparameters, the Decision Tree and KNN models achieved the highest accuracy on the test set.

* Launch Site Trends: KSC LC-39A has the highest success rate, likely due to its historical infrastructure and mission types.

* Payload Impact: Heavier payloads and specific orbits (like LEO) show a higher correlation with successful landings.

## Tech Stack & Tools
* Languages: Python (Pandas, NumPy)

* Databases: SQL (IBM DB2)

* Visualization: Matplotlib, Seaborn, Folium (Geospatial)

* Machine Learning: Scikit-Learn (Logistic Regression, SVM, Decision Tree, KNN)

* Environment: Jupyter Notebooks, VS Code

## Repository Structure
├── data/                   # Processed CSV datasets used for modeling

├── notebooks/              # Sequential Jupyter Notebooks (01-04)

│   ├── 01_Data_Collection.ipynb

│   ├── 02_EDA_and_SQL.ipynb

│   ├── 03_Interactive_Maps.ipynb

│   ├── 04_Machine_Learning.ipynb

├── images/                 # Visualizations and map screenshots

└── README.md               # Main project documentation

## Methodology
1. Data Collection: Sourced data from the SpaceX API and Wikipedia using Web Scraping.
2. Data Wrangling: Cleaned data and created a binary "Class" column (1 = Success, 0 = Failure).
3. Exploratory Data Analysis (EDA): Performed SQL queries and statistical visualization to identify patterns.
4. Interactive Mapping: Used Folium to visualize launch site locations and proximities to infrastructure.
5. Predictive Modeling: Built and optimized four classification algorithms using GridSearchCV.

## Credits & Attribution

This project is the culmination of the IBM Data Science Professional Certificate.

* Templates: Certain utility functions and notebook templates were provided by IBM Skills Network.

* Development: Data cleaning, feature engineering, geospatial analysis, and model hyperparameter tuning were performed independently by Rostyslav.
