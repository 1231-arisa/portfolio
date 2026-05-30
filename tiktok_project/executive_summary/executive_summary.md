# Executive Summary — TikTok Claims Classification Project

## Overview
This project analyzes a TikTok video dataset to understand the differences between **claim** and **opinion** content, identify patterns in user behavior, and explore engagement trends.  
The goal is to prepare the dataset for a future **machine learning model** that classifies videos as claims or opinions.

## Key Findings

### 1. Claim vs. Opinion Distribution
The dataset contains both claim and opinion videos.  
Opinions are slightly more common, but claims still represent a significant portion.  
This indicates that **class balancing** may be necessary when training a classification model.

### 2. Engagement Trends
- Claim videos often show **higher engagement** (likes, shares, comments) relative to their view count.  
- Engagement metrics are **highly skewed**, with a small number of viral videos creating large outliers.  
- Normalized metrics（likes_per_view, shares_per_view, engagement_rate）are more reliable for comparison.

### 3. User Behavior Insights
- Most authors are **not verified**, and the majority are **active** rather than banned.  
- Banned authors occasionally show **unusually high engagement**, suggesting potential patterns related to misinformation or controversial content.  
- Verified status does not guarantee higher engagement, indicating that content type may be more influential than user status.

### 4. Video Characteristics
- Video duration varies widely, from short clips to longer videos.  
- Text length（transcription length）also varies, and longer text may correlate with claim content.  
- These features can be useful predictors in a future classification model.

### 5. Data Quality Observations
Several anomalies were identified:
- Viral outliers with extremely high view counts  
- Videos with very short duration  
- Transcriptions with minimal or no text  
These should be addressed during preprocessing to avoid bias in modeling.

## Conclusion
This exploratory analysis provides a strong foundation for building a **claim classification model**.  
By understanding engagement patterns, user behavior, and video characteristics, we can engineer meaningful features and prepare the dataset for deeper EDA, hypothesis testing, and machine learning.

## Next Steps
- Conduct deeper statistical analysis and hypothesis testing  
- Build and evaluate a baseline classification model  
- Explore NLP techniques using transcription text  
- Improve feature engineering to enhance model accuracy  
