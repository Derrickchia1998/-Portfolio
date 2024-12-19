## Education
Business Administration Finance ( Sept 2018 - Sept 2021 )

## Work Experience

**Data Analyst @ Grof (_March 2024 - Dec 2024_)**
*Identified and resolved issue in ETL pipelines
- Improving data accuracy for over 50% of revenue-related metrics, ensuring reliable insights for decision-making.
*Optimized SQL queries for MRR analysis,
- Incorporating add-ons, one-time charges, and first-time fee, resulting in a 20% reduction in report generation time and enhanced accuracy of recurring revenue forecasts.
*Developed advanced churn and growth rate models
- Accounting for complex scenarios like paused, canceled, and resumed subscriptions, which improved subscription mrr amount accuracy to 100% and supported strategic retention initiatives.
* Automated the generation of KPI reports
- Integrating data from multiple platforms using SQL queries and Python ETL scripts. Consolidated data into a unified dashboard, eliminating the need for manual extraction from disparate platforms and reducing report preparation time by 80%. This enabled management to access up-to-date KPIs in real-time, supporting faster and more informed decision-making.

## Portfolio
### Merchandise Sales Analysis: Driving Insights for Growth
In this project, I analyzed a merchandise sales dataset to uncover patterns, optimize sales strategies, and improve customer satisfaction. The goal was to build a robust data pipeline and create dynamic visualizations to assist stakeholders in making data-driven decisions.

#### Step 1: Data Extraction
The first step involved gathering data from multiple platforms. In a real-world scenario, this data would come from APIs or platform exports. For this project, the data was extracted from a CSV file.

![image](https://github.com/user-attachments/assets/f6b077ed-4a7e-4a69-ba5c-fdc5898e15b1)

#### Step 2: Data Cleaning
After extraction, I checked for missing values and inconsistent entries. For example, some columns had missing customer ages or improperly formatted sales amounts. Cleaning ensured the dataset was accurate and analysis-ready.

![image](https://github.com/user-attachments/assets/37551173-d6b4-4a07-9374-4da52d1b3653)

#### Step 3: Data Transformation
The dataset required transformations to prepare it for deeper analysis. This included formatting dates and restructuring sales amounts. SQL was used for this purpose, as it provides an efficient way to handle large datasets.

![image](https://github.com/user-attachments/assets/487023a5-09e6-48b1-bc94-8ca8de4b1050)

Examples of other subscriptions where government charges or non-recurring charges are excluded when calculating revenue.
![image](https://github.com/user-attachments/assets/7e899bc0-17f2-42df-bd0c-99d899d0137c)

#### Step 4: Load to Database
With the cleaned and transformed data, I loaded it into a cloud-based database (e.g., BigQuery) to enable scalability and efficient querying.

![image](https://github.com/user-attachments/assets/77fdcf53-4f02-4c57-86ea-a02b7f4a181e)

#### Step 5: Dashboard Creation
Finally, I visualized the insights using Superset / Metabase / Lookerstudio. The dashboards displayed key metrics, such as top-performing product categories, customer demographics, and shipping efficiency.

![image](https://github.com/user-attachments/assets/1a170e5f-9380-48cd-9b2d-d1a6925cf882)
##### Key Observations:
- Clothing dominates both total sales (637.2K) and record count (3.7K), indicating its popularity.
- Ornaments are the second most popular, with total sales of 155.8K and a record count of 2.3K.
- Other products contribute minimally to sales (63.5K) and records (1.4K).
- Male buyers significantly outnumber female buyers, contributing 600.3K to total sales versus 256.1K for females.
- Male record count is also higher (5,188) compared to females (2,206).
##### Insights:
- Prioritize marketing and inventory for clothing to capitalize on demand.
- Consider strategies to boost sales in underperforming categories.
- Develop gender-specific campaigns to balance gender contributions.
- Explore why male buyers contribute more to both metrics.
  
![image](https://github.com/user-attachments/assets/555f91bb-c207-4b57-b1b3-14ab95b70b8a)
##### Key Observations:
- Average total sales per age group range between 44.7K to 50.1K, with minimal variation.
- Record counts are consistent across ages, showing no significant drop-off with increasing age.
##### Insights:
- The even distribution suggests a broad age appeal.
- Further segmentation could help uncover more granular insights.

![image](https://github.com/user-attachments/assets/a60360c6-0574-4165-9248-3534669a56b9)
##### Key Observations:
- Sales fluctuate slightly but remain within the range of 66.1K to 80.7K across the months.
- May 2024 shows the highest sales peak, while November 2024 has a sharp drop.
##### Insights:
- Analyze seasonal trends or promotional events affecting May's peak.
- Address potential causes for the drop in November.
  
![image](https://github.com/user-attachments/assets/5c33c70a-284e-4819-b7a2-20fd2000ec43)
##### Key Observations:
- Male buyers account for 70.1% of sales, with females at 29.9%.
- Domestic shipping contributes more to total sales (54.8%) compared to international shipping (45.2%).
##### Insights:
- Explore reasons for higher male participation.
- Expand international shipping capabilities to grow global sales.
  
![image](https://github.com/user-attachments/assets/bb23f39c-204f-4e40-87de-73c4b5774de4)
##### Key Observations:
- Total sales are highest for age groups 20, 24, and 35.
- Quantity distribution is relatively stable but slightly lower for buyers aged 33 and higher.
##### Insights:
- Age-targeted campaigns could maximize contributions from high-spending groups.
- Investigate why older buyers have lower quantity purchases.

#### Other Analytics
##### Cohort Analysis
- Join table to obtain customer id where t1.order_id = t2.order_id
- Create a column indicating the first purchase date for each customer.
- Calculate how many months have passed since the first purchase for each subsequent transaction.
- Aggregate metrics like revenue, number of purchases, or retention rate for each cohort by time intervals (e.g., months, quarters).

![image](https://github.com/user-attachments/assets/216ee756-8e83-407a-979a-a3b8b171be3c)

##### Cohort Analysis
- Collect product-level data including selling price, COGS, and discounts.
- Ensure overhead or fixed costs (like shipping) are allocated appropriately.
- Calculate gross profit as Selling Price - COGS.
- Add a column for profit margin percentage: (Gross Profit / Selling Price) * 100.
- Analyze profitability by product category, customer segments, or region.

##### Aggregate Profitability by Product / Customer / Time ( monthly ) / Region
![image](https://github.com/user-attachments/assets/c3b024c8-848e-404b-8fb0-c0c10b374649)

