# Walmart_Sales_Analysis
Retail sales analysis of 45 Walmart stores using Python, SQL, statistical testing, Power Query, Power BI to examine store performance, Holiday impact, seasonality and key sales trend.
Project Overview

This project analyzes weekly sales data from 45 Walmart stores to better understand store performance, seasonal trends, holiday sales patterns, and the relationship between sales and selected economic and environmental factors.

I used Python, SQL, statistical testing, and Power BI to explore the data, answer business questions, and present the main findings clearly.

Business Objective

The objective of this project is to identify key patterns in Walmart’s weekly sales performance and determine which factors are most closely associated with changes in sales.

The analysis focuses on:

• Comparing sales performance across stores
• Identifying seasonal and monthly sales patterns
• Measuring the difference between holiday and regular-week sales
• Evaluating which stores experience the largest holiday sales lift
• Examining relationships between weekly sales and temperature, fuel prices, CPI, and unemployment
• Presenting key findings through an interactive Power BI dashboard

Dataset

Source: Kaggle Walmart Dataset
https://www.kaggle.com/datasets/yasserh/walmart-dataset

The dataset contains 6,435 store-week observations across 45 Walmart stores from February 2010 through October 2012.

Key fields include:

• Store
• Date
• Weekly Sales
• Holiday Flag
• Temperature
• Fuel Price
• CPI
• Unemployment

Tools Used

• Python
• Pandas
• SQLite / SQL
• SciPy
• Matplotlib
• Power BI
• Power Query
• DAX

Data Preparation

The dataset was reviewed for data types, missing values, duplicate records, and date formatting before analysis.

The Date field was converted to a proper datetime format to support chronological analysis and SQL date functions.

Additional date-related fields were created in Power BI to support month, year, quarter, and year-month analysis.

Key Analysis

Store Performance

Average and total weekly sales were analyzed across all 45 stores to identify differences in store-level performance.

The results showed that sales performance varies considerably between locations, meaning company-wide averages can hide important differences between individual stores.

Holiday Sales

Holiday weeks recorded higher average weekly sales than regular weeks.

A paired-samples t-test was used to compare each store’s average holiday-week sales with its own average regular-week sales.

The test produced a t-statistic of approximately 9.65 and a p-value below 0.001, indicating a statistically significant difference between holiday and regular-week sales.

This result does not establish that holidays directly caused the increase, since seasonal demand and other business factors may also contribute.

Holiday Sales Lift

Store-level holiday lift was analyzed using both dollar difference and percentage change.

Store 10 recorded the largest absolute increase in average holiday sales, while Store 7 recorded the largest percentage holiday lift.

This shows that holiday demand does not affect every store equally.

Economic and Environmental Factors

Temperature, fuel prices, CPI, and unemployment showed only weak linear relationships with weekly sales.

These results suggest that none of these variables alone explains a large portion of the variation in store sales.

Power BI Dashboard

A two-page Power BI report was created to provide an interactive view of:

• Total sales
• Average weekly sales
• Number of stores
• Number of observed weeks
• Sales trends over time
• Monthly seasonality
• Top-performing stores
• Holiday vs. regular-week sales
• Store-level holiday sales lift

Dashboard Overview

Dashboard Overview

Store and Holiday Analysis

Store and Holiday Analysis

Key Findings

• Store performance varies significantly across the 45 locations.
• Holiday weeks generate higher average weekly sales than regular weeks.
• Holiday sales impact differs considerably by store.
• Seasonal timing appears more informative than the economic and environmental variables available in the dataset.
• Company-wide averages should be interpreted carefully because store-level differences are substantial.

Business Recommendations

The findings suggest that Walmart could benefit from using store-level performance rather than company-wide averages when making operational decisions.

Holiday periods may require additional inventory and staffing, but planning should account for differences between individual stores rather than applying the same strategy across all locations.

Stores with consistently strong holiday lift could be studied further to identify differences in customer demand, local market conditions, promotions, or product mix.

Limitations

This dataset does not include several factors that could influence weekly sales, including:

• Store size
• Product categories
• Promotions and markdowns
• Local demographics
• Competitor activity
• Inventory levels

The statistical relationships identified in this project should therefore be interpreted as associations rather than proof of causation.

Conclusion

This project provided a clearer picture of how Walmart’s weekly sales vary across stores, time periods, and holiday weeks.

Store-level differences and seasonal timing were among the strongest patterns found in the analysis, while the available economic and environmental variables showed relatively weak linear relationships with sales.

Overall, the analysis shows why looking beyond company-wide averages is important when evaluating retail performance. I also gained experience combining SQL, Python, statistical testing, and Power BI within one end-to-end analysis rather than treating each tool as a separate exercise.

Project Files

• Walmart_Store_Performance_and_Holiday_Impact.ipynb — Python, SQL, and statistical analysis
• Walmart_Retail_Sales_Dashboard.pbix — Power BI dashboard
• images/ — dashboard screenshots

Author

Syeda Tasnim Hossain
