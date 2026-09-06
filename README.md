\# Supply Chain Delivery Performance Analysis



An end-to-end data analytics and machine learning project analyzing e-commerce delivery performance to identify late-delivery patterns, operational bottlenecks, financial impact, and key predictors of delivery delays.



The project combines exploratory data analysis, statistical testing, root-cause diagnostics, feature engineering, and predictive modeling to understand why orders are delivered late and how late-delivery risk can be predicted before shipment.



\---



\## Business Problem



The company experienced a high rate of late deliveries, negatively affecting customer experience and profitability.



The objective of this project was to:



\- Analyze overall delivery performance and late-delivery patterns

\- Identify operational factors contributing to delivery delays

\- Quantify the financial impact of delayed orders

\- Identify important predictors of late delivery

\- Build a machine learning model to predict late-delivery risk before shipment

\- Provide data-driven recommendations to improve delivery performance



\---



\## Dataset Overview



| Metric | Value |

|---|---:|

| Orders Analyzed | 172,765 |

| Analysis Period | January 2015 – January 2018 |

| Late Deliveries | 54.71% |

| On-Time Deliveries | 45.29% |

| Profit at Risk from Delayed Orders | $2.1M |

| Total Profit Across Profitable Orders | $7.5M |



\---



\## Tools \& Technologies



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- Imbalanced-learn (SMOTE)

\- Jupyter Notebook



\---



\## Analytical Approach



\### 1. Exploratory Data Analysis



Delivery performance was analyzed across:



\- Shipping Mode

\- Order Region

\- Customer Segment

\- Product Category

\- Department

\- Order Type

\- Payment Status

\- Order Month

\- Order Hour



Time-based analysis was also performed to identify seasonal and hourly patterns in delivery performance.



\### 2. Statistical Analysis



Statistical techniques were used to investigate relationships between late-delivery risk and numerical as well as categorical variables.



The analysis included:



\- Correlation analysis

\- Chi-square testing for categorical variables

\- Statistical significance testing

\- Feature-level comparisons between late and on-time orders



\### 3. Root-Cause Analysis



The analysis identified major operational bottlenecks, particularly across Shipping Mode and Order Region.



\---



\## Key Business Findings



\### Shipping Mode is a Major Bottleneck



Late-delivery rates varied substantially across shipping modes:



| Shipping Mode | Late Delivery Rate |

|---|---:|

| First Class | 100.0% |

| Second Class | 79.8% |

| Standard Class | 39.8% |

| Same Day | 0.0% |



This indicates that shipping mode is strongly associated with delivery performance.



\### Regional Delivery Risk



Central Africa recorded the highest late-delivery rate at approximately 58.7%.



Within this region:



\- First Class deliveries had a 100% late-delivery rate

\- Second Class deliveries had an 82.8% late-delivery rate



This highlights the need for region-specific logistics planning.



\### Financial Impact



Delayed orders represented approximately $2.1M in profit at risk, demonstrating that delivery performance is both an operational and financial concern.



\### Time-Based Patterns



Delivery performance varied across order months and order hours, making time-based variables useful for predictive modeling.



\---



\## Machine Learning



A supervised classification approach was used to predict whether an individual order would be delivered late.



\### Models Compared



Five classification algorithms were evaluated:



1\. Logistic Regression

2\. Decision Tree

3\. Naive Bayes

4\. Random Forest

5\. Gradient Boosting



\### Feature Engineering



The model used features that would be available before shipment, including:



\- Type

\- Scheduled Shipping Days

\- Category Name

\- Customer Segment

\- Department Name

\- Order Region

\- Shipping Mode

\- Order Month

\- Order Hour



Categorical variables were transformed using frequency encoding.



\### Model Training



\- Stratified 80/20 train-test split

\- SMOTE applied only to the training data to address class imbalance

\- Multiple classification models evaluated using performance metrics

\- Feature importance analyzed for the final model



\---



\## Final Model: Random Forest



Random Forest was selected as the final model based on its overall predictive performance.



| Metric | Score |

|---|---:|

| Accuracy | 73.58% |

| Precision | 78.28% |

| Recall | 74.57% |

| F1-Score | 76.38% |

| ROC-AUC | 82.26% |



The model achieved an ROC-AUC of 0.82, indicating good ability to distinguish between late and on-time deliveries.



\---



\## Important Predictors



Feature importance analysis identified the following variables among the most influential predictors of late delivery:



1\. Order Hour

2\. Scheduled Shipping Days

3\. Order Region

4\. Order Month

5\. Shipping Mode



These features provide useful signals for identifying delivery risk before an order is shipped.



\---



\## Business Recommendations



\### 1. Review High-Risk Shipping Modes



Investigate the operational causes behind the extremely high late-delivery rates for First Class and Second Class shipments.



\### 2. Implement Region-Specific Logistics Strategies



Prioritize regions such as Central Africa for additional logistics capacity, carrier evaluation, and route optimization.



\### 3. Introduce Pre-Shipment Risk Prediction



Use the predictive model to flag high-risk orders before shipment so that corrective action can be taken proactively.



\### 4. Optimize Scheduled Shipping



Use historical delivery patterns and scheduled shipping days to improve delivery planning and reduce unrealistic delivery commitments.



\### 5. Monitor High-Risk Time Periods



Use month and hour-level patterns to anticipate periods of increased delivery risk and allocate resources accordingly.



\---



\## Project Workflow



Data Collection  

↓  

Data Cleaning \& Preparation  

↓  

Exploratory Data Analysis  

↓  

Statistical Analysis  

↓  

Root-Cause Diagnostics  

↓  

Feature Engineering  

↓  

Model Training  

↓  

Model Comparison  

↓  

Random Forest Selection  

↓  

Feature Importance Analysis  

↓  

Business Recommendations



\---



\## Project Files



| File | Description |

|---|---|

| `Supply\_Chain\_Analysis.ipynb` | Complete data analysis, visualization, statistical analysis, feature engineering, and machine learning workflow |

| `Supply\_Chain\_Delivery\_Performance\_Report.docx` | Detailed project report containing methodology, findings, model evaluation, and recommendations |

| `.gitignore` | Specifies large datasets and model artifacts excluded from version control |



> Note: The original dataset and trained model files are not included in this repository because of their large file sizes. The notebook contains the complete analysis and modeling workflow.



\---



\## Conclusion



This project demonstrates an end-to-end approach to solving a real-world supply chain problem using data analytics and machine learning.



The analysis identified a 54.71% late-delivery rate and approximately $2.1M in profit at risk, while highlighting Shipping Mode, Order Region, and time-based factors as important drivers of delivery risk.



The final Random Forest model achieved an ROC-AUC of 0.82, demonstrating its potential to support proactive identification of high-risk orders before shipment.



Overall, the project combines business analysis, statistical reasoning, data visualization, and predictive modeling to translate operational data into actionable business insights.



\---



\## Author



\*\*Renu Nadar\*\*



MSc Statistics | Data Analytics \& Machine Learning

