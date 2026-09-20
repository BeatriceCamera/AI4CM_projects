# AI for Communication & Marketing — Customer Analytics

A collection of three data-driven marketing projects exploring **customer segmentation, churn prediction, and customer lifetime value (CLTV)** through statistical analysis, machine learning, and actionable communication strategies. The projects follow the customer lifecycle from understanding **who customers are**, to predicting **who may leave**, and finally estimating **which customers are worth retaining and investing in**.

## Projects

### 1. Customer Segmentation & Communication Strategy

Customer analytics project combining **exploratory data analysis, RFM segmentation, and unsupervised learning** to identify meaningful customer groups and translate them into targeted communication strategies.

- **Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, missingno, scikit-learn, scipy
- **Methods:** EDA, Feature Engineering, RFM Analysis, K-Means Clustering, PCA, Silhouette Analysis

#### Overview

The project analyzes customer demographic, transactional, channel, and campaign data to understand what drives customer value and how different customer groups behave. After data cleaning and exploratory analysis, customers are segmented using two complementary approaches:

1. **RFM segmentation**, based on Recency, Frequency, and Monetary value.
2. **K-Means clustering**, incorporating broader demographic, behavioral, channel, and product-preference information.

The goal is not only to identify high- and low-value customers, but to convert these patterns into differentiated marketing actions.

#### Key Insights

- Income emerges as the strongest driver of customer spending.
- Child-free customers spend substantially more, particularly on Wines and Meat.
- Omnichannel customers generate higher average value.
- High-value inactive customers form a strategically important reactivation segment.
- RFM and clustering capture complementary aspects of customer behavior rather than producing identical groups.

The analysis results in actionable customer segments including **Champions, Sleeping Giants, Loyal Mid-Spenders, Price-Sensitive Customers, At-Risk Customers, and New/Occasional Buyers**, each associated with specific communication channels, messages, and KPIs.

---

### 2. Churn Prediction & Retention Strategy

Machine learning project focused on **predicting customer churn and transforming churn probabilities into targeted retention actions**.

- **Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, SHAP, missingno
- **Models:** Logistic Regression, Random Forest, XGBoost
- **Methods:** Classification, Hyperparameter Tuning, ROC-AUC Analysis, Lift Analysis, Feature Importance, SHAP

#### Overview

The project develops an end-to-end churn prediction pipeline from customer demographic, engagement, satisfaction, and transactional data.

Three classification models are evaluated:

1. **Logistic Regression**
2. **Random Forest**
3. **XGBoost**

XGBoost is further optimized using randomized hyperparameter search and stratified cross-validation. Rather than evaluating the models only through predictive metrics, the project also uses **lift analysis** to determine how churn scores can be operationalized when marketing resources are limited.

#### Key Insights

- Churn is strongly concentrated in the early stages of the customer lifecycle.
- Customers filing complaints show substantially higher churn risk.
- The combination of low tenure and complaints identifies an especially vulnerable customer group.
- XGBoost achieves the strongest predictive performance among the evaluated models.
- Targeting the highest-risk customers allows retention campaigns to cover most potential churners while reducing campaign size.

Model insights are translated into three retention interventions:

- **Early Lifecycle Engagement**
- **Complaint Service Recovery**
- **Product Category Activation**

Each strategy defines a target audience, timing, intervention, and KPI, connecting predictive modelling directly to CRM decision-making.

---

### 3. Customer Lifetime Value & Retention Strategy

Customer value modelling project comparing **probabilistic CLTV modelling and machine learning** to support both financial planning and individual customer targeting.

- **Language:** Python
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost, lifetimes
- **Models:** BG/NBD, Gamma-Gamma, XGBoost Regressor
- **Methods:** CLTV Prediction, RFM Analysis, Probabilistic Modelling, Regression, Customer Value Segmentation

#### Overview

The project investigates a central marketing question:

> How much is the customer base worth, and which customers should receive retention investment?

Using the Olist e-commerce dataset, multiple relational data sources are integrated into a customer-level transaction history and analyzed through two complementary modelling approaches.

### BTYD Probabilistic Framework

The **BG/NBD model** estimates future purchase frequency and customer survival probability, while the **Gamma-Gamma model** estimates future monetary value among repeat purchasers.

Together, they provide an interpretable probabilistic Customer Lifetime Value framework.

### XGBoost Approach

An **XGBoost Regressor** is trained to estimate future customer value from behavioral and transactional features.

Unlike the monetary component of the BTYD framework, the machine-learning model can assign customer-level scores across a broader customer base, making it particularly useful for ranking and campaign targeting.

#### Key Insights

- Customer value is highly concentrated among a relatively small share of repeat buyers.
- Most customers make only one purchase, creating a highly sparse future-revenue prediction problem.
- BTYD and XGBoost provide complementary information rather than acting as direct substitutes.
- Probabilistic modelling offers interpretable forecasting for repeat customers, while machine-learning scores support granular CRM targeting.
- Combining predicted CLTV with BG/NBD survival probability identifies valuable customers whose future engagement is at risk.

The resulting strategy distinguishes between:

- **Win-Back Targets** — high predicted value but low probability of remaining active
- **Retention Priorities** — high-value customers who remain engaged
- **Growth Segments** — established customers with opportunities for cross-selling and category expansion

---

## From Data to Marketing Action

Across the three projects, machine learning is treated not only as a predictive tool but as a support system for **marketing decision-making**.

The complete workflow moves through three levels:

**Understand → Predict → Prioritize**

- **Customer Segmentation:** Who are our customers and how should we communicate with them?
- **Churn Prediction:** Who is likely to leave and when should we intervene?
- **Customer Lifetime Value:** Which customers justify additional retention and marketing investment?

The final objective is to connect analytical outputs with concrete decisions about **audience, message, channel, timing, and marketing investment**.

## Repository Contents

- `LabExam_1.ipynb` — Customer Segmentation & Communication Strategy
- `LabExam_2.ipynb` — Churn Prediction & Retention Strategy
- `LabExam_3.ipynb` — Customer Lifetime Value & Retention Strategy
- Supporting datasets used throughout the analyses
- Presentation decks summarizing the strategic findings

## Author

**Beatrice Camera**

B.Sc. Artificial Intelligence  
University of Pavia · University of Milan · University of Milano-Bicocca
