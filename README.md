# -task4-Data-Storytelling-Statistical-Validation
# 📊 Task 4 – Data Storytelling & Statistical Validation

## Overview

This project is the final phase of my Data Analytics Internship, where I transformed raw sales data into meaningful business insights using Data Storytelling and Statistical Validation.

The objective was to combine previous data cleaning, exploratory data analysis (EDA), and dashboard findings into a clear business narrative and validate a key insight using a statistical test.

---

## Objectives

- Analyze cleaned sales data to identify business insights.
- Present findings through an engaging business story.
- Validate a key finding using an Independent Two-Sample T-Test.
- Provide actionable business recommendations.

---

## Tools & Technologies

- Python
- Pandas
- Matplotlib
- SciPy
- Jupyter Notebook
- Microsoft PowerPoint
- GitHub

---

## Project Structure

```
Task4_DataStorytelling/
│
├── Cleaned_Data.xlsx
├── task4_analysis.ipynb
├── Task4_Professional_DarkBlue_Presentation.pptx
├── Business_Summary.xlsx
├── graphs/
│   ├── monthly_sales.png
│   ├── category_sales.png
│   ├── city_sales.png
│   └── top_products.png
└── README.md
```

---

## Exploratory Data Analysis (EDA) Highlights

- Electronics generated the highest sales revenue.
- Bangalore recorded the highest sales among all cities.
- Monthly sales showed a positive growth trend.
- A small number of top-selling products contributed significantly to total revenue.

---

## Business Story

The analysis revealed that the business is experiencing steady growth, with Electronics emerging as the strongest-performing category. High-performing cities present opportunities for targeted marketing campaigns, while increasing inventory for best-selling products can further improve sales performance.

---

## Hypothesis Testing

### Business Question

**Do Electronics products generate higher sales than Fashion products?**

### Hypotheses

- **H₀ (Null Hypothesis):** There is no significant difference between Electronics and Fashion sales.
- **H₁ (Alternative Hypothesis):** Electronics sales are significantly higher than Fashion sales.

### Statistical Test

- **Test Used:** Independent Two-Sample T-Test
- **Library:** `scipy.stats.ttest_ind`

### Example Result

| Metric | Value |
|--------|-------|
| Test | Independent T-Test |
| P-value | Less than 0.05 |
| Conclusion | Statistically Significant |

**Business Interpretation:** Since the p-value is below 0.05, the null hypothesis is rejected, indicating that Electronics sales are significantly higher than Fashion sales.

---

## Business Recommendations

- Increase inventory for Electronics products.
- Focus marketing efforts on high-performing cities like Bangalore.
- Promote top-selling products through targeted campaigns.
- Monitor monthly sales trends to support future business planning.

---

## Key Learnings

- Data Cleaning and Preparation
- Exploratory Data Analysis (EDA)
- Business Storytelling
- Hypothesis Testing using Python
- Statistical Interpretation
- Professional Presentation Skills
- GitHub Project Documentation

---

## Author

**Kamani Kumari**

Data Analytics Internship – Task 4

---

⭐ If you found this project helpful, feel free to explore the repository and connect with me on LinkedIn.
