# TikTok_Claim_ML
TikTok Report System: Machine Learning Models (Random Forest &amp; XGBoost)


# TikTok: Claims vs. Opinions - Machine Learning for Classifying User Reports
<div style="text-align: center;"><img src="tik_tok_logo2.jpg" alt="Example Image" width="200"/></div>

## Project Overview

This project aims to enhance TikTok's report system by developing a machine learning model capable of distinguishing between user reports that classify content as either a "claim" or an "opinion." The dataset consists of user engagement metrics, such as video views, likes, shares, and comments, which were analyzed and used as features for classification modeling. This project involved training and evaluating Random Forest and XGBoost models to optimize classification performance, with the best model selected based on precision, recall, and F1-score.

## Business Understanding

The ability to effectively categorize user reports is essential for TikTok's content moderation system, ensuring misinformation is effectively managed while maintaining fair content classification. This project supports the platform’s goal of improving automated content moderation by leveraging machine learning models to distinguish factual claims from subjective opinions, enhancing both user experience and compliance with content policies.

## Data Understanding

The dataset contains various user engagement metrics, including:
- Video views
- Likes
- Comments
- Shares
- Downloads

Data limitations include missing values and a right-skewed distribution in variables such as view and like counts, which required preprocessing before model training.

Exploratory Data Analysis (EDA) revealed:
- Over 200 null values across seven different columns.
- A highly imbalanced distribution of videos classified as "opinions" compared to "claims."
- Right-skewed distributions for engagement metrics, necessitating appropriate data transformations.

## Modeling and Evaluation

The project followed a structured approach with five key steps:

1. **Preliminary Analysis** – Initial data exploration and cleaning. 
    - [Analysis](https://github.com/franeze/TikTok_Claim_ML/blob/main/1_Preliminary_Analysis/tiktok_preliminary_analysis.ipynb)
    - [Executive Summary](https://github.com/franeze/TikTok_Claim_ML/blob/main/1_Preliminary_Analysis/Preliminary%20data%20Analysis%20-%20Executive%20summary.pdf)
2. **Exploratory Data Analysis (EDA)** – Identifying patterns, distributions, and missing data.

    - [Analysis](https://github.com/franeze/TikTok_Claim_ML/blob/main/2_EDA/TikTokEDA.ipynb)
    - [Executive Summary](https://github.com/franeze/TikTok_Claim_ML/blob/main/2_EDA/executive%20summary.pdf)
4. **Hypothesis Testing** – T-tests were conducted to validate assumptions about user engagement and video performance. Specifically, the analysis examined whether TikTok videos posted by verified accounts receive significantly more views than those posted by unverified accounts.
    - [Analysis](https://github.com/franeze/TikTok_Claim_ML/blob/main/3_Hypothesis_testing/Hypothesis_testing.ipynb)
    - [Executive Summary](https://github.com/franeze/TikTok_Claim_ML/blob/main/3_Hypothesis_testing/Executive_summary.pdf)
6. **Logistic Regression** – Establishing a baseline classification model.
    - [Analysis](https://github.com/franeze/TikTok_Claim_ML/blob/main/4_Regression_Model/Tik_Tok_Regression_model.ipynb)
    - [Executive Summary](https://github.com/franeze/TikTok_Claim_ML/blob/main/4_Regression_Model/executive_summary.pdf)
7. **Random Forest & XGBoost** – Training and evaluating advanced machine learning models.
    - [Analysis](https://github.com/franeze/TikTok_Claim_ML/blob/main/5_Random_Forest_and_XGBoost/Tik_Tok_RandomForest_XGBoost.ipynb)
    - [Executive Summary](https://github.com/franeze/TikTok_Claim_ML/blob/main/5_Random_Forest_and_XGBoost/executive_summary.pdf)

Evaluation metrics included:
- **Precision, Recall, and F1-score** to measure classification accuracy.
- **Confusion Matrix** to assess misclassification rates.
- **ROC-AUC Score** to evaluate model performance.

Results:
- Both models performed exceptionally well, with Random Forest slightly outperforming XGBoost in recall (0.999 vs. 0.998).
- The champion model primarily relied on user engagement metrics to classify videos.
- Due to near-perfect performance, no immediate feature engineering was required, though additional features such as the number of reports per author could further refine results.

## Conclusion

The machine learning model developed in this project significantly improves TikTok’s report classification system by accurately distinguishing between claims and opinions. Future work may include:
- Incorporating additional features, such as the number of times a video has been reported.
- Enhancing data preprocessing techniques to address potential biases.
- Deploying the model in a live environment for real-time classification and continuous learning.

This project demonstrates the power of machine learning in content moderation and highlights how data-driven approaches can improve user experience and platform integrity.

