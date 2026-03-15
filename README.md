# 🚀 Winning Space Race with Data Science
**IBM Data Science Professional Certificate - Capstone Project**

**Author:** Wélbster Florentino Labat Uchôas  
**Date:** December 2025  

![SpaceX Falcon 9](https://images.unsplash.com/photo-1541185933-ef5d8ed016c2?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80) 

## 📋 Executive Summary
SpaceX has revolutionized the space industry with its reusable rockets. While a standard rocket launch costs upwards of $165 million, SpaceX can do it for $62 million, primarily because they recover and reuse the Falcon 9 first stage. 

**The Goal of this Project:** Predict if the Falcon 9 first stage will land successfully. By determining the likelihood of a successful landing, we can estimate the true cost of a launch. This predictive insight allows competing companies to bid more effectively against SpaceX for satellite launch contracts.

---

## 🛠️ Methodology & Tech Stack
This project was built following a complete Data Science methodology:

1. **Data Collection:** 
   * Extracted data using the **SpaceX REST API**.
   * Web Scraped historical Falcon 9 launch records from **Wikipedia** using `BeautifulSoup`.
2. **Data Wrangling:** Filtered data, handled missing values, and applied One-Hot Encoding for categorical variables.
3. **Exploratory Data Analysis (EDA):**
   * Used **SQL** to query metrics (total payload, launch outcomes, booster versions).
   * Visualized trends using `Matplotlib` and `Seaborn`.
4. **Interactive Visual Analytics:**
   * Built interactive maps with **Folium** to analyze launch site proximity to coastlines and highways.
   * Developed a dynamic web dashboard using **Plotly Dash** to filter success rates by payload mass and launch site.
5. **Predictive Analysis (Machine Learning):**
   * Standardized data and split it into training (80%) and testing (20%) sets.
   * Built, tuned (via `GridSearchCV`), and evaluated 4 classification models using `Scikit-Learn`: Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN).

---

## 📊 Key Insights & Results

* **Technological Maturity:** The success rate of Falcon 9 landings has trended significantly upward since 2013, stabilizing at a near-perfect rate in recent years.
* **Launch Site:** **KSC LC-39A** is the most active and reliable launch pad, contributing to ~41.7% of all successful launches.
* **Payload Mass vs. Orbit:** Heavier payloads (>8,000 kg), often associated with established mission profiles like Starlink or ISS resupply (LEO/Polar orbits), show predominantly successful landings.
* **Geographical Advantage:** Launch sites are deliberately located near coastlines (0.8–1.5 km) to maximize safety for populated areas during early flight stages.

### Machine Learning Performance
All four classification models performed exceptionally well, achieving an accuracy of **83.33%** on the test data. 
* **Best Model:** The **Decision Tree** model is highlighted for its high interpretability.
* **Risk Analysis:** The Confusion Matrix revealed occasional *False Positives* (predicting a successful landing when it actually crashes). In a business context, this is the riskiest error, as it could lead to underestimating launch costs by assuming booster reuse when it is actually lost.

---

## 📁 Repository Structure & Notebooks

Here you can find all the code developed during this project. Click the links to view the Jupyter Notebooks:

| Phase | Description | Link |
|-------|-------------|------|
| **Data Collection** | API Data Extraction | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/jupyter-labs-spacex-data-collection-api.ipynb) |
| **Data Collection** | Web Scraping Wikipedia | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/jupyter-labs-webscraping.ipynb) |
| **Data Wrangling** | Cleaning and Formatting | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/labs-jupyter-spacex-Data%20wrangling%20.ipynb) |
| **EDA - Visualization** | Matplotlib & Seaborn Charts | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/edadataviz%20.ipynb) |
| **EDA - SQL** | SQLite Queries | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/jupyter-labs-eda-sql-coursera_sqllite%20%20.ipynb) |
| **Map Visualization** | Folium Interactive Maps | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/lab_jupyter_launch_site_location%20.ipynb) |
| **Dashboard** | Plotly Dash App (Python script) | [View Code](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/spacex-dash-app%20.py) |
| **Machine Learning** | Classification & Evaluation | [View Notebook](https://github.com/welbster/Applied-Data-Science-Capstone/blob/main/SpaceX_Machine%20Learning%20Prediction_Part_5%20.ipynb) |

*Full Presentation Deck:* [View PDF Presentation (https://drive.google.com/file/d/11JSHNP3iaRg2d4OWvpJr9FiZXeYvB5_R/view?usp=sharing)]


---

## 🏅 Acknowledgements
This project was developed as the final Capstone for the **IBM Data Science Professional Certificate** offered on Coursera.

---
*If you have any questions or want to connect, feel free to reach out via [LinkedIn](https://www.linkedin.com/in/w%C3%A9lbster-uch%C3%B4as/).*
