# SpaceX Falcon 9 First Stage Landing Prediction
**IBM Data Science Professional Certificate Capstone Project**

**Author:** Yousef Buhamad  
**GitHub Repository:** [IBM-Data-Science-Capstone](https://github.com/YousefBuhamad/IBM-Data-Science-Capstone)

---

## Executive Summary

The primary objective of this project is to predict whether the first stage of a SpaceX Falcon 9 rocket will land successfully. SpaceX reuses the first stage of its rockets to drastically cut the cost of space launches—charging around $62 million per launch compared to competitors' $165+ million. By accurately forecasting landing success based on public launch parameters, competing launch providers can better estimate true mission costs and bidding strategies.

### Key Results & Findings
- **Data Overview:** Analyzed 90 launches across key launch sites: KSC LC-39A, SLC-40, and VAFB SLC-4E.
- **Top Performing Site:** **KSC LC-39A** led all launch pads with a **77.3%** success rate.
- **Overall Success Rate:** Across the entire historical dataset, the landing success rate reached **66.67%**, including 41 successful autonomous spaceport drone ship landings (`True ASDS`).
- **Machine Learning Performance:** All evaluated classifiers (Logistic Regression, SVM, Decision Tree, and K-Nearest Neighbors) achieved a **83.33% accuracy** on the test set, with Decision Trees demonstrating superior speed and simplicity during hyperparameter tuning.

---

## Project Architecture & Methodology

```text
1. Data Collection  --->  2. Wrangling & EDA  --->  3. Interactive Analysis  --->  4. Machine Learning
   - SpaceX REST API         - One-Hot Encoding         - Folium Maps               - Logistic Regression
   - Web Scraping (BS4)      - SQL Queries              - Plotly Dash App           - SVM, KNN, Decision Tree
