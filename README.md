# TikTok Truth Serum: Classifying Content on TikTok

## Project Overview 📋
This project develops a **machine learning model** to classify TikTok videos as either **claims** or **opinions** based on engagement metrics. The goal is to improve content moderation and ensure compliance with TikTok's terms of service by identifying videos likely to contain claims, which may need prioritized review. This work is part of the **Google Advanced Data Analytics Capstone Project**.

## Problem Statement 😩
Accurately classifying TikTok videos as claims or opinions is essential for moderating content and ensuring compliance with platform guidelines. This classification prioritizes videos for review, reducing the spread of misinformation.

## Workbook Navigation 📂

- **01_data_initial_exploration.ipynb**  
  Initial data inspection, organization, and preparation with basic visualizations to understand the dataset.

- **02_data_visualization.ipynb**  
  In-depth data exploration with numerous charts to analyze distributions, identify outliers, and uncover patterns.

- **03_hypothesis_testing.ipynb**  
  Hypothesis testing to explore the relationship between `video_view_count` and `verified_status`, including two-sample t-tests and verification steps.

- **04_Logistic_Regression.ipynb**  
  Development of a logistic regression model to predict `verified_status`, featuring one-hot encoding, feature selection (e.g., exclusion of `video_like_count` due to high correlation), model evaluation, and interpretation.

## Dataset 🔢
The dataset includes TikTok video metadata such as:
- **Identifiers**: `video_id` (unique video identifier)
- **Content Features**: `video_duration_sec`, `video_transcription_text`, `verified_status` (author’s verification status)
- **Engagement Metrics**: `video_view_count`, `video_like_count`, `video_share_count`, `video_download_count`, `video_comment_count`

### Data Preparation
- **Handling Missing Values**: Imputed missing values in key columns.
- **Feature Engineering**: Created new features like `likes_per_view` and `shares_per_view` to enrich the data.

## Methodology 🛠️
1. **Data Exploration**: Explored data characteristics using summary statistics and visualizations (see `01_data_initial_exploration.ipynb` and `02_data_visualization.ipynb`).
2. **Feature Transformation**: Applied log transformations to skewed features and selected important features based on exploratory findings.
3. **Hypothesis Testing**: Conducted hypothesis tests, including a two-sample t-test, to examine relationships between variables (see `03_hypothesis_testing.ipynb`).
4. **Model Selection and Evaluation**: Built and evaluated models — **Random Forest**, **XGBoost**, and **Logistic Regression** — using metrics like **Precision**, **Recall**, **F1-score**, and **Accuracy** (detailed in `04_Logistic_Regression.ipynb`).

### Future Considerations
- **Naive Bayes Model**: Naive Bayes is considered for future implementation due to its relevance for certain target variables and its potential in handling categorical data effectively for customer segmentation or engagement analysis.

### Model Interpretation
- **Feature Importance**: Key features influencing predictions included `video_view_count`, `video_like_count`, and `video_share_count`.
- **Behavioral Insights**: Longer videos and higher engagement metrics were strongly associated with claim videos, suggesting that these videos are more likely to contain claims.

## Model Performance 🔩
- **Random Forest**: Precision 69%, Recall 66%, F1-score 66%
- **XGBoost**: Precision 70%, Recall 68%, F1-score 68%
- **Logistic Regression**: Precision 68%, Recall 53%, F1-score 61%, Accuracy 67%

## Results and Insights 📊
- **Claim vs. Opinion Trends**: Claim videos generally show higher engagement metrics compared to opinion videos.
- **Moderation Strategy**: Prioritizing high-engagement videos for review could improve content moderation efficiency.

## Conclusion 💡
- **Recap**: The project successfully developed a model to classify TikTok videos as claims or opinions, supporting content moderation.
- **Recommendations**: Further refine the model with additional data and features, and deploy it in a production environment for real-time classification.

## Next Steps 🔜
1. **Model Extension**: Incorporate additional data sources and features to enhance accuracy.
2. **Performance Monitoring**: Regularly evaluate and update the model to ensure sustained effectiveness.
3. **User Training**: Equip moderation teams with training to effectively leverage the classification system.

## Appendices 📑
- **Code and Queries**: The complete code and queries are provided in the accompanying Jupyter Notebooks.
- **Additional Visualizations**: Supplementary charts and tables supporting findings are included in the project documentation.

--- 

This README now mentions Naive Bayes as a potential future enhancement without adding unnecessary detail, keeping it clean and professional.
### Additional Charts and Tables
- Additional visualizations and tables supporting the findings are included in the project documentation.
  ![image](https://github.com/user-attachments/assets/9c04cafe-1189-4e82-aac9-4a4e9b5e1a2e)
---

author: Myckland Matthew
email: myckland.matthew@gmail.comn
