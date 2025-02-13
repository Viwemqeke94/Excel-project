# Excel-project
Insurance Data Analysis Dashboard
 Key Insights from the Dashboard
📊 Summary Statistics
Average Insurance Price: $18,244.35
Average Age: 29.10 years
Average BMI: 39.70 (indicating a high BMI level)
These summary cards provide a quick glance at key metrics, helping to identify trends in insurance pricing.

💰 Price per Body Weight Category
Normal Weight → $15,644.67
Overweight → $23,118.75
Grand Total → $18,244.35
This suggests that overweight individuals tend to pay higher insurance premiums.

👶 Insurance Price by Number of Children
0 children → $15,120.83
1 child → $12,912.50
2 children → $21,805.38
3 children → $24,374.44
The data shows an increasing trend in insurance price as the number of dependents increases.

🚬 Smoking vs Non-Smoking
Smokers (23.91%) pay higher premiums than Non-Smokers (76.09%)
The pie chart visually compares these two groups, showing the significant impact of smoking on insurance costs.
📈 Trend & Distribution Analysis
Age Distribution: A bar chart displays how insured individuals are spread across different age brackets.
Insurance Price Trend: A line chart highlights how insurance costs tend to rise with age.
2️⃣ Data Analysis Techniques Used
✅ Data Cleaning
Before analysis, the dataset was cleaned to remove inconsistencies, ensuring accuracy in calculations and visualizations.

✅ Formulas & Functions Used
📌 IF & COUNTIF Functions
Used for:

Categorizing BMI & Age


Edit
=IF(D2<25, "Normal Weight", IF(D2<30, "Overweight", "Obese"))
This formula classifies individuals based on their BMI.

Counting Specific Conditions



=COUNTIF(F:F, "Yes")
This counts the number of smokers in the dataset.

🔍 XLOOKUP for Data Retrieval
Used to dynamically fetch insurance prices based on:

BMI Category Lookup


Edit
=XLOOKUP(D2, BMI_Category_Table[Category], BMI_Category_Table[Avg_Insurance_Price])
This retrieves the average insurance price for a given BMI category.

Age Bracket Lookup


Edit
=XLOOKUP(B2, Age_Group_Table[Age], Age_Group_Table[Category])
This helps categorize individuals into the correct age group.

3️⃣ Advanced Excel Features Implemented
✅ Slicers for Interactive Filtering
Slicers were added for Smoking Status, Gender, and Age Categories, allowing users to filter the dashboard dynamically.

✅ Conditional Formatting for Better Insights
Applied to highlight high insurance prices and categorize data visually.
Used in tables and charts to enhance readability.
