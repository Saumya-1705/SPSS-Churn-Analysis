# Predictive Customer Churn Analytics using IBM SPSS Modeler

## 📌 Project Overview
This project builds an end-to-end predictive analytics classification pipeline using IBM SPSS Modeler to predict customer churn in the telecommunications sector. The objective is to identify high-risk churn customers and guide proactive retention strategies.

## 🛠️ IBM SPSS Modeler Stream Architecture
The pipeline consists of the following sequential steps:
1. **Data Ingestion (`Var. File` Node):** Loaded raw customer records (`telecom_churn.csv`).
2. **Type Mapping (`Type` Node):** Designated `Churn` as the categorical Target (Flag/Nominal) and configured input feature attributes.
3. **Data Partitioning (`Partition` Node):** Split data into training and testing partitions to evaluate model generalization.
4. **Model Training (`C5.0` Node):** Trained a decision tree classification model.
5. **Model Evaluation (`Analysis` Node):** Evaluated predictive accuracy and generated a confusion matrix.

## 📂 Repository Contents
- `telecom_churn.csv` — Raw dataset used for the project.
- `spss_stream.str` — Native IBM SPSS Modeler visual pipeline file.
- `presentation.pdf` — Final project slide deck.
- `screenshots/` — Visual records of the SPSS Modeler pipeline canvas and evaluation results.

## 📊 Results & Business Insights
- Identified key churn drivers such as high customer service call counts and unfavorable pricing tiers.
- The C5.0 model successfully classified high-risk churn segments, offering actionable retention pathways for business decision-makers.
