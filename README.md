# Telco-Customer-Churn-Analysis-and-Prediction
In the fiercely competitive landscape of the telecommunications industry, retaining customers is of paramount importance for sustainable growth and profitability. Customer churn, the phenomenon where subscribers terminate their services, poses a significant challenge to telecom companies. Understanding the factors that drive customer churn and developing effective strategies to predict and mitigate it is crucial for telecom operators to optimize their business operations.

This project aims to delve into the intricate world of telecom customer churn analysis and prediction through supervised machine learning. By leveraging the power of data analytics and machine learning, I seek to uncover valuable insights from historical customer data and build models that can accurately predict potential churners.

## Project Overview
The main goal of this project is to understand customer churn patterns and build a predictive model to identify customers who are likely to leave the service. The project is divided into four main phases:

### 1. Data Preparation and Data Warehousing
- Started with a raw CSV dataset containing telecom customer information.  
- Used **SQL Server** to create a **Data Warehouse**.  
- Designed **Fact and Dimension tables** to organize the data in a star schema.  
- Loaded the data into the warehouse using **SSIS (SQL Server Integration Services)**.

**DWH Structure:**  
<img width="748" height="519" alt="DWH Schema" src="https://github.com/user-attachments/assets/99bfe7b8-3902-4684-93ce-ad461579db23" />

### 2. ETL Process with SSIS
- Built ETL packages to extract, transform, and load data from the raw CSV to the data warehouse.  
- Ensured data consistency and applied necessary transformations.
**SSIS ETL Example:**
<img width="814" height="384" alt="ETL_SSIS_DIMENSIONS" src="https://github.com/user-attachments/assets/02fb2ae7-d552-4975-adb2-c9e51f195e2e" />
<img width="490" height="419" alt="ETL_SSIS_FACT" src="https://github.com/user-attachments/assets/4fc0ba94-4d75-4c0e-8863-af83199c17d3" />

  


### 3. Data Visualization with Power BI
- Connected the data warehouse to **Power BI**.  
- Built interactive **dashboards** to explore customer behavior, churn rates, and key metrics.  
- Visualizations include trends, distributions, and comparisons between churned and retained customers.

**Power BI Dashboard**  
<img width="914" height="501" alt="Screenshot (108)" src="https://github.com/user-attachments/assets/42920bd0-6fa9-41f6-a9cc-f87f957cc594" />
<img width="902" height="512" alt="Screenshot (110)" src="https://github.com/user-attachments/assets/09020e64-4043-4ad7-9fd6-1cee7d14a495" />
<img width="906" height="518" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/1be1575f-f92b-4209-8cc3-3d5123c67275" />
<img width="902" height="512" alt="Screenshot (110)" src="https://github.com/user-attachments/assets/6fdb56c6-174c-43d7-8703-b51d9c695b8f" />




### 4. Machine Learning Model
- Prepared the data for modeling by selecting relevant features.  
- Built a **Machine Learning model** to predict customer churn.  
- Evaluated the model using metrics such as precision, recall, and accuracy.  
- The model helps identify at-risk customers and enables proactive retention strategies.

**Machine Learning Model:**  
<img width="539" height="568" alt="Screenshot (115)" src="https://github.com/user-attachments/assets/febfdd76-737b-4618-8bc9-fc2c31b0f5b3" />


## Technologies Used
- **SQL Server** – Data storage and warehouse creation  
- **SSIS** – ETL processes for loading data into the warehouse  
- **Power BI** – Data visualization and dashboards  
- **Python / Machine Learning libraries** – Model building and evaluation  

## Executive Summary
This analysis of customer churn for a telecommunications company reveals a critical churn rate of 26.86%, representing 1,796 lost customers. The primary drivers of churn are identified as customer service issues, specific payment methods, and the lack of long-term contracts. Customers with Month-to-Month contracts, those who make frequent customer service calls, and those using Paper Checks for payment are at the highest risk. Immediate, targeted retention strategies are recommended to mitigate further revenue loss.

## Insights / Findings
### High Overall Churn Rate
The company's overall churn rate is 26.86%. This indicates that over a quarter of the customer base is leaving, representing a significant threat to revenue and growth.

### Primary Churn Reasons are Customer Service Related
The most frequent reason for churn is "Courtesy," followed closely by "Attitude" and "Disastritis" (likely "Dissatisfaction"). This points to a significant issue with the quality of customer service and support interactions, which is the single biggest driver of customer attrition.

### Contract Type is a Major Predictor of Churn
The data clearly shows that customers on Month-to-Month contracts are significantly more likely to churn compared to those on longer-term contracts. This highlights the fragility of the customer base without long-term commitments.

### Service Usage and Plan Analysis

International Plan: A small segment of customers (9.74%) have the International Plan. The churn rate among this group appears to be a critical area for investigation.

Unlimited Data Plan: The majority of customers (67.21%) have the Unlimited Data Plan, suggesting it is a key offering.

Usage Patterns: Churned customers show distinct usage patterns, including lower average monthly GB downloads and a different profile for local and international calls compared to retained customers.

### Customer Service Interaction is a Key Indicator
There is a strong correlation between the number of customer service calls and the likelihood of churn. Customers who churn have a higher average number of customer service calls, indicating that unresolved issues or service frustrations are a primary cause of leaving.

### Payment Method Correlation
Customers who use Paper Checks as a payment method show a higher propensity to churn compared to those using electronic methods like Credit Cards or Direct Debit. This may be related to convenience or demographic factors.

### Geographic Concentration of Churn
Churn is not evenly distributed. States like West Virginia (WV) and Ohio (OH) have the highest number of churned customers, suggesting potential regional issues with network quality, local competition, or marketing effectiveness.

## Recommendations
### Revamp Customer Service Training & Processes
Immediately address the top churn reasons by implementing enhanced training programs focused on courtesy, empathy, and effective problem-solving for customer service representatives.

### Incentivize Long-Term Contracts
Launch a campaign to migrate Month-to-Month customers to one-year or two-year contracts by offering perks, discounted hardware, or price locks. This is the most effective lever to reduce churn.

### Proactive Retention for High-Risk Customers
Create an alert system for customers who make more than 2-3 customer service calls in a billing cycle. Proactively reach out to these customers with dedicated support and potential offers to resolve their issues before they decide to leave.

### Promote Electronic Payment Methods
Incentivize customers to switch from Paper Checks to Direct Debit or Credit Card payments through a small monthly discount or a one-time bonus, thereby reducing the churn risk associated with this payment method.

### Conduct Regional Analysis in High-Churn States
Initiate a deep-dive analysis into the market conditions in top churn states like WV and OH. Investigate local competitor offers, network performance, and customer sentiment to develop targeted regional retention strategies.

