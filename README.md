# E-Commerce Purchase Prediction: Identifying High-Intent Buyers


## Overview This project predicts which website visitors are most likely to make a purchase, helping businesses improve conversion rates and marketing efficiency.

---

## The Business Problem

E-commerce websites attract many visitors, but only a small percentage actually complete a purchase. This leads to inefficient marketing spending and missed revenue opportunities. Identifying potential buyers early allows companies to target them more effectively and increase conversions.


## The Data

We analyzed a dataset of over 12,000 user sessions, capturing user behavior such as time spent on pages, traffic source, visitor type, and browsing patterns. The dataset includes both purchasing and non-purchasing users, allowing us to identify patterns that influence buying decisions.

## Key Discoveries

- Users who spend more time on product-related pages are more likely to purchase  
- Returning visitors show higher engagement and conversion behavior  
- Certain traffic sources lead to higher purchase probability  
- User engagement metrics like bounce rate strongly influence buying decisions  



## Visualizing the Story

![Model Insights](chart.png)


## Prediction Model

The Logistic Regression model achieved approximately 83% accuracy, outperforming Gaussian Naive Bayes (64%). However, the model tends to predict non-purchase outcomes more often, meaning it misses some actual buyers despite strong overall accuracy.

## Recommendations

1. Improve targeting of potential buyers using predictive insights.
Action: Use the predictive model to identify users likely to purchase and focus marketing efforts (emails, ads, offers) on them.
Evidence: The model shows clear patterns in distinguishing purchasing vs non-purchasing users, even though some buyers are currently missed.
Impact: Better targeting can increase conversion rates and reduce wasted marketing spend on uninterested users.

2. Reduce missed opportunities by improving model sensitivity.
Action: Adjust the model to better capture potential buyers (reduce false negatives), even if it slightly increases false positives.
Evidence: The confusion matrix shows a high number of false negatives, meaning many actual buyers are not being identified.
Impact: Capturing more potential buyers can directly increase revenue, even if it leads to some additional marketing costs.

3. Focus on engaging undecided users with personalized strategies.
Action: Implement personalized recommendations, discounts, or retargeting campaigns for users who show interest but do not convert.
Evidence: The model struggles to identify all purchasing users, indicating a segment of users who are close to converting but not fully engaged.
Impact: Converting even a small portion of these users can significantly boost sales.

4. Continuously improve model performance with better features and tuning.
Action: Experiment with additional models, feature engineering, and parameter tuning to improve prediction quality.
Evidence: While Logistic Regression outperformed Naive Bayes, it still fails to identify many buyers.
Impact: A more accurate model can improve decision-making and lead to higher long-term profitability.

## Tools & Techniques

Python | Pandas | Scikit-Learn | Matplotlib | Seaborn | Gaussian Naive Bayes | Google Colab

---

*This project was completed as part of ISOM 835: Predictive Analytics at Suffolk University's
Sawyer Business School.*
