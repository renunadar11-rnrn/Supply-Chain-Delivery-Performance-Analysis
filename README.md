\# Supply Chain Delivery Performance Analysis



\## Project Overview



An end-to-end analysis of e-commerce delivery performance to identify late-delivery drivers, operational bottlenecks, their financial impact, and opportunities for improvement.



\## Business Problem



The company faced a high rate of late deliveries, affecting customer experience and profitability. The objective was to analyze delivery performance, identify key causes of delays, quantify their financial impact, and build a predictive model to flag high-risk orders before shipment.



\## Objectives



\- Analyze overall delivery performance and late-delivery patterns

\- Identify operational bottlenecks and root causes of delays

\- Quantify the financial impact of late deliveries

\- Build a machine learning model to predict late-delivery risk

\- Provide data-driven recommendations for improving delivery performance



\## Tools \& Technologies



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- SMOTE

\- Jupyter Notebook



\## Key Findings



\- Analyzed \*\*172,765 orders\*\*

\- \*\*54.71%\*\* of orders were delivered late

\- Late deliveries represented approximately \*\*$2.1M in profit at risk\*\*

\- \*\*Shipping Mode\*\* was identified as the strongest operational bottleneck

\- First Class shipments had a \*\*100% delay rate\*\*

\- Second Class shipments had a \*\*79.8% delay rate\*\*

\- Seasonal peaks were observed during \*\*August, September, and December\*\*



\## Statistical Analysis



The analysis included:



\- Exploratory Data Analysis

\- Pearson correlation analysis

\- Chi-square tests of independence

\- Feature engineering

\- Bottleneck detection

\- Root cause analysis

\- Time-based delay analysis



\## Machine Learning



Five classification algorithms were evaluated:



1\. Logistic Regression

2\. Decision Tree

3\. Naive Bayes

4\. Random Forest

5\. Gradient Boosting



Categorical variables were frequency encoded and the training data was balanced using SMOTE.



\### Final Model



\*\*Random Forest\*\* was selected as the final model based on its overall performance.



\- Accuracy: \*\*73.58%\*\*

\- Recall: \*\*74.57%\*\*

\- F1-Score: \*\*76.38%\*\*

\- ROC-AUC: \*\*0.82\*\*



The model uses pre-shipment features to identify orders that are at higher risk of late delivery.



\## Business Recommendations



\- Audit First Class and Second Class shipping performance

\- Implement predictive alerts for high-risk orders

\- Address payment-processing bottlenecks

\- Develop additional capacity plans for seasonal demand

\- Review shipping-mode assignment logic

\- Investigate high-delay departments and regions



\## Project Files



```text

Supply-Chain-Delivery-Performance-Analysis/

│

├── Supply\_Chain\_Analysis.ipynb

├── Supply\_Chain\_Delivery\_Performance\_Report.docx

├── README.md

└── .gitignore



\### Conclusion



The analysis identified shipping mode, scheduled delivery windows, regions, and time-based factors as important contributors to late deliveries. The Random Forest model provided a data-driven approach for identifying high-risk orders before shipment and supporting proactive operational intervention.

