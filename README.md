# 📊 Sales Uplift Analysis for Online Retail Store

## 📌 Objective
The primary goal of this project was to assess the effectiveness of a marketing campaign by estimating the incremental revenue generated during the campaign period. Using historical transaction data from an online retail store, the analysis aimed to compare actual sales during the campaign with forecasted sales had the campaign not occurred.

---

## 📂 Data Overview
- **Time period covered:** January 1, 2021 to September 7, 2021
- **Total records:** 250 daily observations
- **Key columns:**
  - `date`: Transaction date
  - `customer_id`: Unique ID per customer
  - `product_id`: Unique ID per product
  - `quantity`: Number of products sold
  - `unit_price`: Price per product
  - `revenue`: Total transaction revenue
  - `marketing_campaign`: Boolean flag indicating if the transaction occurred during the marketing campaign
- ✅ No missing values
- ✅ Continuous daily sales data (no gaps)

---

## 🧪 Exploratory Data Analysis (EDA)

### 📈 Revenue Trends
- Daily revenue shows a notable increase starting around the marketing campaign launch date.
- A vertical dashed line was plotted to indicate the campaign start, showing a visible uplift.

### 📦 Revenue Distribution
- A boxplot comparison revealed that the **median revenue** during the campaign period was significantly higher.
- More high-value revenue days (outliers) appeared during the campaign.

### 🔁 Customer Behavior
- **Average revenue** per day increased by a factor of **~2.25** during the marketing campaign.
- **Average quantity sold** also increased compared to non-campaign days.
- This indicates both more frequent and larger transactions during the marketing period.

---

## 🧠 Causal Impact Modeling

### 🔮 Forecasting Method
- A **Facebook Prophet** model was trained using **pre-campaign data** only.
- The model forecasted daily revenue during the **post-campaign** period, simulating what would have happened without the marketing intervention.

### 🆚 Forecast vs Actual Revenue
The following results were obtained:

| Metric | Value |
|:------|:-----|
| 📈 Total Actual Revenue (Post-Campaign) | \$37397.29 |
| 📉 Total Predicted Revenue (No Campaign) | \$8033.13 |
| 🔼 Estimated Uplift | \$29364.16 |
| 🔼 Uplift Percentage | 365.54% |


---

## 🖼️ Visualization

A time series plot was generated showing:
- Historical revenue (gray line)
- Actual revenue during campaign (green line)
- Forecasted revenue without campaign (red dashed line)
- Campaign start (vertical dotted line)

---

## 📋 Conclusion
- The marketing campaign had a **clear and measurable positive effect** on daily revenue.
- Actual revenue **exceeded expected revenue** significantly during the campaign period.
- The **uplift percentage** confirms that the marketing effort successfully boosted sales beyond normal expectations.
- Using causal forecasting models like Prophet provides an objective and statistically grounded way to validate marketing ROI.

---

## 🏆 Final Status
- ✅ Data Cleaning
- ✅ EDA
- ✅ Causal Modeling
- ✅ Uplift Quantification
- ✅ Business Insights

**Project Completed Successfully! 🚀**

---
