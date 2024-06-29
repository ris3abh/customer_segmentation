# Predicting Family Size Using Deep Learning for Enhanced Business Insights

## Project Overview

This project aims to accurately predict family size based on customer attributes and purchasing behavior data. Understanding family size is crucial for businesses to gain valuable insights into consumer behavior, preferences, and purchasing patterns. These insights can inform marketing strategies, product development, and resource allocation decisions, ultimately leading to more personalized and effective business practices.

## Significance

Family size is a key demographic factor influencing consumer needs, spending habits, and decision-making processes. Accurate predictions of family size can help businesses better understand their target audience and tailor their offerings, promotions, and services accordingly.

## Objectives

1. **Data Preparation:** 
   - Handle missing values
   - Encode categorical variables
   - Scale features

2. **Model Exploration:**
   - Experiment with different deep learning architectures (e.g., RNNs, Bidirectional RNNs)

3. **Model Optimization:**
   - Fine-tune hyperparameters
   - Apply regularization techniques
   - Optimize model performance

4. **Model Evaluation:**
   - Use metrics like accuracy, precision, recall, and F1-score

5. **Deployment Strategy:**
   - Integrate the trained model into business decision-making processes and operational systems

## Data Source

The dataset is sourced from a marketing campaign for a Portuguese banking institution, containing various customer attributes, product details, and previous campaign responses. [Dataset Link](https://www.kaggle.com/datasets/rodsaldanha/arketing-campaign)

## Data Description

- **IDYear_Birth:** Customer's year of birth
- **Education:** Customer's education level
- **Marital_Status:** Customer's marital status
- **Income:** Customer's income
- **Kidhome:** Indicator for presence of kids at home
- **Teenhome:** Indicator for presence of teenagers at home
- **Dt_Customer:** Customer acquisition date
- **Recency:** Recency of last purchase or activity
- **MntWines:** Amount spent on wines
- **NumWebVisits:** Number of web visits
- **AcceptedCmp[1-5]:** Indicators for campaign acceptance
- **Complain:** Indicator for complaints
- **Z_CostContact:** Cost of contacting the customer
- **Z_Revenue:** Customer's revenue
- **Response:** Campaign response

##Data Exploration
Marital_Status:

- 8 distinct categories, with "Married" being the most common
Inconsistencies noted (e.g., "Absurd" and "YOLO")
Education:

- 5 distinct categories, with "Graduation" being the most common
Income Distribution: Right-skewed with a long tail

- Recency: Bimodal distribution

- Customer Tenure: Heavily skewed towards short tenures

- Age Distribution: Bimodal, representing younger individuals and older adults

## Model Development
Architecture Exploration:
- Recurrent Neural Networks (RNNs)
- Bidirectional RNNs
Fine-Tuning:
- Adjust hyperparameters
- Apply regularization techniques
- Performance Optimization:
- Evaluate using accuracy, precision, recall, and F1-score

##Deployment Strategy
Integrate the trained model into the business’s decision-making processes and operational systems to enhance marketing campaigns, product development, customer segmentation, and resource allocation.

## Benefits
- Targeted Marketing Campaigns: Tailor campaigns and promotions based on family size for better engagement and effectiveness
- Product Development and Inventory Management: Develop products catering to different family sizes and optimize inventory levels
- Customer Segmentation and Personalization: Enhance segmentation strategies and deliver personalized experiences
- Resource Allocation and Operational Efficiency: Optimize resource allocation to better serve the needs of different family sizes

## Results

<h1>Model Performance Summary</h1>
    <table>
        <thead>
            <tr>
                <th>Model</th>
                <th>Metric</th>
                <th>Value</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td rowspan="2">Bidirectional RNN</td>
                <td>Test Loss</td>
                <td>0.09454477578401566</td>
            </tr>
            <tr>
                <td>Test Accuracy</td>
                <td>0.9729119539260864</td>
            </tr>
            <tr>
                <td>RNN</td>
                <td>Accuracy</td>
                <td>0.9774266481399536</td>
            </tr>
            <tr>
                <td>Bidirectional RNN</td>
                <td>Accuracy</td>
                <td>0.9729119539260864</td>
            </tr>
        </tbody>
    </table>
