# Chocolate Sales Analysis  
Advanced Big Data and Data Mining – Bi-term 2  
Student Name: Banoj Kumar Jena  
Deliverable: Week 2 – Data Collection, Cleaning, and Exploration  

---

Project Overview  
This project is part of the Advanced Big Data and Data Mining course, designed to walk through the complete data mining lifecycle using real-world datasets. In Deliverable 1, we focus on data collection, cleaning, and exploration using a chocolate sales dataset. This stage sets the foundation for later deliverables including feature engineering, predictive modeling, and unsupervised learning.

---

Dataset Summary  

Dataset: Chocolate Sales  
Source: Provided internally  
Records: Approximately 1,000 rows  
Attributes:
- sales_person: Name of the sales representative  
- country: Sales region  
- product: Type of chocolate  
- date: Date of transaction  
- amount: Total sale amount  
- boxes_shipped: Number of units shipped  

Dataset Justification  
This dataset is well-suited for sales and performance analytics, regression analysis such as predicting revenue, classification such as identifying high versus low sales categories, and clustering such as segmenting by product or region. It includes both numeric and categorical features, has sufficient volume, and contains realistic variability for practical data mining tasks.

---

Data Cleaning and Preprocessing Steps  

1. Column Renaming  
   Column names were standardized to lowercase with underscores for consistency and code readability.

2. Type Conversion  
   The 'date' column was converted to datetime format.  
   The 'amount' and 'boxes_shipped' columns were converted to numeric using coercion to handle invalid entries.

3. Missing Values  
   Missing or invalid dates and numeric values were handled using dropna to ensure clean records.

4. Duplicates  
   Duplicate records were identified and removed to ensure unique transactions.

5. Noise and Outliers  
   Outliers were visualized using boxplots for both 'amount' and 'boxes_shipped'. These were noted for future analysis but not removed at this stage.

---

Exploratory Data Analysis (EDA)  

1. Correlation Analysis  
   A strong positive correlation was found between 'amount' and 'boxes_shipped', confirming expected sales behavior.

2. Country-Level Insights  
   Certain countries contributed significantly more to total revenue, indicating regional disparities in sales.

3. Product-Level Insights  
   Some chocolate products such as Truffle and Dark Chocolate generated higher revenue and appear more popular among customers.

4. Seasonal Trends  
   Monthly analysis revealed cyclical demand patterns, suggesting seasonality in chocolate sales.

5. Outlier Detection  
   Visual inspection revealed a few high-value transactions that may represent special cases or bulk orders. These were retained for modeling.

---

Key Insights  

- Sales are highly concentrated in a few regions and products.  
- There is a strong correlation between quantity shipped and revenue.  
- Some countries underperform and could be targeted with regional marketing efforts.  
- Seasonality plays a role in sales patterns and should be accounted for in forecasting and planning.  

---

Challenges Faced  

- Date formats were inconsistent and required careful conversion.  
- Some records contained null or non-numeric values in key fields such as amount and boxes shipped.  
- There was variability in categorical values, which may require encoding and grouping in future phases.  

---

Next Steps for Future Deliverables  

- Perform feature engineering such as extracting month, weekday, or quarter from the date field.  
- Encode categorical variables using one-hot or label encoding.  
- Build regression models to predict sales amount based on product, country, and date features.  
- Apply clustering techniques to group similar products or regions.  
- Develop classification models to segment high and low performing sales.  

---

Repository Structure  

- Deliverable1.ipynb: Jupyter Notebook with code, analysis, and visualizations  
- Chocolate Sales.csv: Raw dataset used in this analysis  
- README.md: Summary of the project, dataset, cleaning steps, and key findings  

---

Submission Notes  

This repository contains all the required components for Deliverable 1. The dataset was thoroughly cleaned, analyzed, and visualized. All insights are documented and supported by visual and statistical evidence. The project is ready for review and serves as the foundation for future modeling and evaluation tasks in the data mining process.

