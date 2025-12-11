# Chicago Traffic Crash Analysis and Predictive Modeling

## 🎯 Project Overview

This project provides a comprehensive analysis of traffic crash data from the **Chicago Data Portal**. The primary goals are to:

1.  **Analyze Trends:** Conduct Exploratory Data Analysis (EDA) to identify key patterns and factors contributing to traffic incidents in Chicago.
2.  **Predict Severity:** Develop and utilize machine learning models to predict the severity of crashes based on contributing factors.
3.  **Support Public Safety:** Generate data-driven insights to inform traffic regulation policies, guide urban planning, and support proactive safety measures.

## 💾 Data Source and Technology

* **Data Source:** Chicago Data Portal - Traffic Incidents Dataset.
* **Data Size:** Approximately 470 MB, covering 48 features.
* **Key Technology:** The analysis leverages **PySpark** for scalable data loading, cleaning, and processing, which is essential for handling large-scale city data efficiently.

## 💻 Methodology

The analysis follows a standard data science pipeline:

1.  **Data Loading and Setup:** Loading the raw data using Spark.
2.  **Data Cleaning:** Handling null values, performing type casting, and ensuring data consistency.
3.  **Exploratory Data Analysis (EDA):** Investigating crash frequency based on temporal (Day of the Week, Month), environmental (Weather, Lighting), and infrastructure factors (Posted Speed Limit).
4.  **Machine Learning:** Training predictive models (details on specific models are in the notebook) to classify or predict crash severity.
5.  **Insights Generation:** Drawing conclusions for actionable safety interventions.

## 📈 Key Insights & Findings

### 1. External Factors & Crash Severity

* **Weather Conditions:** Strong correlations exist between specific weather conditions and the frequency of traffic incidents.
* **Lighting Conditions:** Lighting conditions (e.g., darkness, daylight, twilight) significantly correlate with crash occurrences and severity.
* **Speed Limits:** Analysis of average posted speed limits at incident locations helps determine the correlation between speed and injury-related crashes.

### 2. Temporal & Infrastructure Trends

* **Day of the Week:** Investigation into the frequency of incidents across different days helps pinpoint high-risk days, likely related to traffic volume or behavioral patterns.
* **High-Risk Zones:** Geospatial analysis helps identify specific intersections or areas with consistently high crash rates.

## 💡 Conclusion & Future Scope

The analysis successfully provided critical, data-driven insights to improve road safety in Chicago.

### **Actionable Recommendations**

* **Targeted Interventions:** Interventions (e.g., increased patrol, road maintenance) can be focused on high-risk zones and specific times of the week.
* **Regulation Policy:** Findings related to speed limits and lighting can inform traffic regulation and infrastructure improvement policies.

### **Future Scope**

* **Predictive Analysis:** Enhance the predictive model to support proactive safety measures, such as adjusting speed limits in high-risk areas or improving lighting in vulnerable zones based on real-time data and prediction.
* **Feature Engineering:** Further explore feature engineering, particularly with geospatial and temporal components, to enhance model accuracy.

## 📂 Project Files

| File Name | Description |
| :--- | :--- |
| `Traffic_Crashes_Final (1).ipynb` | The Jupyter Notebook containing the full analysis pipeline: PySpark data processing, EDA using SQL queries, and machine learning implementation. |
| `Traffic Crash Analysis on Chicago Dataset 1 (1).pptx` | The presentation summarizing the project objectives, data methodology, key EDA insights, and final conclusions/future scope. |

## ⚙️ Requirements

To run the analysis in `Traffic_Crashes_Final (1).ipynb`, you will need an environment capable of running **PySpark** (e.g., Databricks, Google Colab with Spark integration, or a local Spark setup).

Required Libraries:

```bash
pyspark
pandas
matplotlib
