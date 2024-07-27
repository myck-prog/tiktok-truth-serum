# TikTok Data Analysis Project

## Introduction 📋
This project aims to develop a machine learning model to classify TikTok videos as claims or opinions based on various engagement metrics. The goal is to improve content moderation and ensure compliance with TikTok's terms of service by accurately identifying videos that are more likely to make claims.

## Problem Statement 😩
Accurately classifying TikTok videos as claims or opinions is crucial for moderating content and ensuring compliance with the platform's terms of service. This classification helps prioritize videos for review and prevents the spread of misinformation.

## Dataset 🔢
### Data Sources
The dataset consists of TikTok video metadata, including view counts, like counts, share counts, and more. The data is sourced from TikTok's internal databases and includes both verified and unverified accounts.

### Data Dictionary
- `video_id`: Unique identifier for each video
- `video_duration_sec`: Duration of the video in seconds
- `video_transcription_text`: Text transcription of the video
- `verified_status`: Whether the author is verified or not
- `author_ban_status`: Author's ban status
- `video_view_count`: Number of views
- `video_like_count`: Number of likes
- `video_share_count`: Number of shares
- `video_download_count`: Number of downloads
- `video_comment_count`: Number of comments

### Data Cleaning and Preparation
- **Handling Missing Values**: Imputed missing values in columns like `video_view_count`, `video_like_count`, etc.
- **Data Type Conversions**: Ensured correct data types for each column.
- **Feature Engineering**: Created new features such as `likes_per_view`, `comments_per_view`, and `shares_per_view`.

## Methodology 🛠️
### Data Collection and Loading
The data was loaded into a Pandas dataframe for analysis. Initial exploration was conducted to understand the size, shape, and composition of the dataset.

### Data Cleaning and Preparation
- Inspected the data for missing values and outliers.
- Cleaned and transformed the data to ensure consistency and accuracy.

## Exploratory Data Analysis 🔍
- **Initial Data Exploration**: Used `head()`, `info()`, and `describe()` to understand the dataset.
- **Visualizations**: Created histograms, box plots, and scatter plots to visualize distributions and relationships.
- **Insights**: Identified trends and patterns, such as higher engagement levels for claim videos.

## Feature Engineering 🔧
- **Transformed Features**: Applied log transformation to skewed features.
- **Selected Important Features**: Based on EDA, selected features like `video_view_count`, `video_like_count`, and `video_share_count`.

## Model Development 🔩
### Model Selection
Tested various models including Random Forest, XGBoost, and Logistic Regression. Selected models based on their performance metrics.

### Model Evaluation
- **Random Forest**: 
  - Precision: 69%
  - Recall: 66%
  - F1-score: 66%
- **XGBoost**: 
  - Precision: 70%
  - Recall: 68%
  - F1-score: 68%
- **Logistic Regression**: 
  - Precision: 65%
  - Recall: 62%
  - F1-score: 63%

### Model Interpretation
- **Feature Importance**: Key features influencing the predictions included `video_view_count`, `video_like_count`, and `video_share_count`.
- **Behavioral Insights**: Longer videos and higher engagement metrics were strongly associated with claim videos, indicating that such videos are more likely to contain claims.

## Results and Insights 📊
- **Summary of Findings**: Claim videos tend to have higher engagement metrics compared to opinion videos.
- **Actionable Insights**: Prioritize high-engagement videos for review to improve content moderation efficiency.

## Conclusion 💡
- **Recap**: The project successfully developed a model to classify TikTok videos as claims or opinions, aiding in content moderation.
- **Recommendations**: Further refine the model with additional data and features, and deploy the model in a production environment for real-time classification.

## Future Work 🧭
- **Extend the Model**: Incorporate new data and features to enhance model accuracy.
- **Fine-tune the Model**: Continuously retrain the model with new data.
- **Enhance the UI**: Improve the user interface for better accessibility and usability.

## Appendices 📑
### Queries or Code
- Detailed code and queries used in the analysis are provided in the accompanying Jupyter Notebooks and scripts.

### Additional Charts and Tables
- Additional visualizations and tables supporting the findings are included in the project documentation.
  ![image](https://github.com/user-attachments/assets/9c04cafe-1189-4e82-aac9-4a4e9b5e1a2e)


---

# Executive Summary

## Project Overview
The TikTok data team aims to develop a machine learning model to assist in the classification of claims for user submissions. This project involves hypothesis testing, model development, and user engagement analysis to create an effective classification system.

## Key Insights
- **Statistical Testing**: Verified accounts tend to have higher video view counts compared to unverified accounts.
- **Model Performance**: The Random Forest model achieved the highest recall score, making it the best choice for identifying claim videos.
- **Feature Importance**: `video_view_count`, `video_like_count`, and `video_share_count` were identified as the most important features for predicting claim status.

## Model Evaluation
- **Random Forest**: 
  - Precision: 69%
  - Recall: 66%
  - F1-score: 66%
- **XGBoost**: 
  - Precision: 70%
  - Recall: 68%
  - F1-score: 68%
- **Logistic Regression**: 
  - Precision: 65%
  - Recall: 62%
  - F1-score: 63%

## Model Interpretation
- **Feature Importance**: Key features influencing the predictions included `video_view_count`, `video_like_count`, and `video_share_count`.
- **Behavioral Insights**: Longer videos and higher engagement metrics were strongly associated with claim videos, indicating that such videos are more likely to contain claims.

## Results and Insights
- **Engagement Trends**: Videos with higher view counts and engagement metrics are more likely to be classified as claims.
- **Actionable Insights**: Implementing this model can help prioritize high-engagement videos for review, improving the efficiency of content moderation on the platform.

## Recommendations
- **Model Refinement**: Continue to refine the model with additional data and features.
- **Deployment**: Deploy the model in a production environment to classify videos in real-time.
- **User Interface Enhancement**: Improve the user interface to make it more accessible and user-friendly.

## Next Steps
1. **Extend the Model**: Incorporate new data and features to enhance model accuracy.
2. **Monitor Model Performance**: Regularly evaluate the model to ensure it remains effective over time.
3. **User Training**: Provide training for users to effectively utilize the classification system.

---

This structure ensures that your project is comprehensive, easy to navigate, and highlights critical aspects of your analysis, making it easier for hiring managers and data managers to understand your work and assess your skills.
