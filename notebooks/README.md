**SpaceX Project: Notebooks Directory**

This folder contains the step-by-step Jupyter Notebooks used to complete the SpaceX Falcon 9 Landing Prediction project. The notebooks are organized numerically to reflect the data science lifecycle, from initial ingestion to final predictive modeling.


**Execution Sequence**

01_Data_Collection_and_Wrangling.ipynb
* Purpose: Acquire and clean the dataset.

* Key Tasks:
  * Extracting launch data from the SpaceX API and supplement with web-scraped data.

  * Handling missing values and identifying the "Class" column (1 for successful landings, 0 for unsuccessful).

  * Exporting the processed data to dataset_part_1.csv.


02_EDA_SQL_and_Visualization.ipynb
* Purpose: Explore the data to find underlying trends and success drivers.

* Key Tasks:
  * Executing SQL queries to analyze payload distribution and launch site performance.
  * Creating scatter plots and bar charts using Matplotlib/Seaborn to visualize success rates over time and across different orbits.


03_Interactive_Visual_Analytics.ipynb
* Purpose: Perform geospatial analysis of launch sites.

* Key Tasks:
  * Building an interactive map with Folium.
  * Adding Marker Clusters to identify high-density success zones.
  * Implementing the Haversine formula to calculate proximities to critical infrastructure (coastlines, highways, and cities).


04_Machine_Learning_Prediction.ipynb
* Purpose: Build and evaluate classification models.

* Key Tasks:
  * Feature engineering and data standardization using StandardScaler.
  * Hyperparameter tuning via GridSearchCV.
  * Comparing the performance of Logistic Regression, SVM, Decision Tree, and K-Nearest Neighbors (KNN).
