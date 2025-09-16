# 📊 Bank Customer Churn Analysis Using Microsoft Excel

## 📌 Project Overview
This project investigates why customers have been leaving a commercial bank in recent months. Using Microsoft Excel, I analyzed customer demographics, financial attributes, product usage, and satisfaction indicators to uncover patterns and drivers of churn. The analysis highlights which customer groups are most at risk and provides actionable recommendations to improve retention.

---

## 🗂️ Dataset
- **Source**: Excel file  
- **Size**: 9,992 records, 18 fields  
- **Key Variables**:  
  - **CustomerId**: Unique identifier  
  - **Age / AgeGroup**: Customer age and derived grouping (Young, Middle-aged, Old, Very Old)  
  - **Geography**: Country of residence (Spain, France, Germany)  
  - **Gender**: Male/Female  
  - **Tenure**: Years with the bank  
  - **Balance**: Account balance  
  - **NumOfProducts**: Number of products owned  
  - **CreditScore**: Credit rating of the customer  
  - **HasCrCard**: Ownership of a credit card (1 = Yes, 0 = No)  
  - **IsActiveMember**: Active membership status (1 = Yes, 0 = No)  
  - **EstimatedSalary**: Approximate salary of the customer  
  - **SatisfactionScore**: Rating of bank services (1–5)  
  - **CardType**: Gold, Platinum, Diamond, Silver  
  - **Complaints**: Whether customer lodged complaints (1 = Yes, 0 = No)  
  - **Exited**: Churn status (1 = Yes, 0 = No)  

---

## 🛠️ Tools and Skills Used
- Microsoft Excel  
- PivotTables & PivotCharts  
- Conditional Formatting  
- XLOOKUP, INDEX-MATCH, Text Functions  
- CORREL function for correlation analysis  
- Dashboard design for churn insights  

---

## 🧹 Data Cleaning & Preparation
- Validated **CustomerId** column for duplicates (none found).  
- Checked for missing values (none observed).  
- Standardized column formats for accuracy (Boolean, numeric, text).  
- Created **AgeGroup** to simplify age analysis:  
  - 18–34 → Young  
  - 35–49 → Middle-aged  
  - 50–70 → Old  
  - 70+ → Very Old  

---

## 🔍 Exploratory Data Analysis (EDA)
The exploratory phase focused on uncovering patterns between customer attributes and churn behavior.  

**Approach**  
- PivotTables and PivotCharts used for grouping and churn percentages.  
- CORREL function tested relationships between churn and numeric variables (age, credit score, salary, balance).  
- Conditional formatting flagged high-risk profiles.  
- AgeGroup derived for better demographic segmentation.  

**Preliminary Observations**  
- Customers in **Germany** churned more than those in Spain and France.  
- **Middle-aged (35–49)** and **older customers** showed higher churn rates.  
- Customers with **low satisfaction scores** and **complaints** were highly likely to churn.  
- Customers with **one product** were more loyal, while those with 3+ products showed very high churn (above 80%).  
- **Diamond cardholders** churned more than Gold cardholders, suggesting dissatisfaction with premium offerings.  

---

## 📊 Data Visualization
Key insights were presented through an Excel dashboard. Add your screenshots here:

- **Churn by Geography**  
  ![Churn by Geography](visuals/churn_by_geography.png)

- **Churn by Age Group**  
  ![Churn by Age](visuals/churn_by_age.png)

- **Satisfaction Score vs Churn**  
  ![Satisfaction vs Churn](visuals/satisfaction_vs_churn.png)

- **Product Engagement vs Churn**  
  ![Product Engagement](visuals/product_engagement.png)

*(Save your Excel dashboard screenshots in a `/visuals` folder and link them as shown above.)*

---

## 💡 Findings & Insights
- **Age**: Strong positive correlation with churn (r ≈ 0.50). Older customers are more likely to leave.  
- **Geography**: Germany had significantly higher churn compared to Spain and France.  
- **Balance**: High-balance customers churned more, signaling a risk of losing profitable clients.  
- **Credit Score**: Lower credit scores correlated with higher churn.  
- **Card Type**: Diamond cardholders had a churn rate of ~21.8%, higher than Gold (~19.3%).  
- **Complaints**: Customers who lodged complaints were far more likely to churn.  

---

## ✅ Recommendations
1. **Retention Programs for Older & High-Balance Customers** – loyalty perks, dedicated managers, and exclusive offers.  
2. **Localized Strategy for Germany** – research causes of dissatisfaction and design market-specific interventions.  
3. **Reassess Premium Card Benefits** – redesign Diamond card offerings to increase perceived value.  
4. **Strengthen Complaint Resolution** – implement faster response times and proactive follow-ups.  
5. **Enhance Onboarding for New Customers** – structured welcome programs and early engagement initiatives.  

---

## 📌 Conclusion
The analysis uncovered the main drivers of churn: customer age, geography, balance, product type, and dissatisfaction through complaints. Germany, older customers, and premium product holders were particularly vulnerable.  

By implementing targeted retention strategies, strengthening customer support, and reassessing product value, the bank can reduce churn and protect long-term profitability.  

---

## 🔮 Future Work
- Develop a **predictive churn model** using Python or Power BI.  
- Automate churn dashboards for real-time monitoring.  
- Incorporate qualitative customer feedback for deeper insights.  

---

📂 Full report available in [`docs/Bank_Customer_Churn_Analysis_Report.docx`](docs/Bank_Customer_Churn_Analysis_Report.docx)  

👤 **Author**: Abdulrazak Jubril  
📌 **Keywords**: Data Analytics, Excel Dashboard, Customer Churn, Business Insights
