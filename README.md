# Train-Rides-Analysis--Power-BI-Project
## Project Overview
The objective is to analyze train rides data, focusing on station performance, ticket sales, and revenue trends using Power BI.
The dataset includes departure station details, delayed trip reasons, ticket class distribution, and revenue over time. The insights from this analysis can help stakeholders optimize operations and improve customer experience.

# Questions (KPIs)
To derive valuable insights, I focused on the following key performance indicators (KPIs):
•Total rides by departure station – Identifying the busiest stations.
•Delayed trips by reason – Understanding the primary causes of delays.
•Ticket sales distribution – Comparing standard vs. first-class ticket sales.
•Revenue trends over time – Tracking sales performance across different periods.

# Process
## Data Cleaning & Preparation
•Removed duplicates and null values.
•Standardized column names for consistency.
•Transformed date formats for accurate time-based analysis.
## Data Analysis & Visualization (Power BI)
•Column Chart for total rides by departure station.
•Bar Chart to display delayed trips categorized by reasons.
•Pie Chart for ticket class distribution.
•Line Chart to analyze revenue trends over time.
•Tree Map to visually compare station ride counts.
## DAX Measures Used  
Average Delay Time = AVERAGEX ('Fact Transactions', [Delay Minutes]) 

Delayed Trips by Reason = COUNTROWS (FILTER ('Fact Transactions', 'Fact Transactions'[Reason for Delay] <> "No Delay")) 

Ticket Type Sales = COUNT ('Fact Transactions'[Ticket ID]) 

Total Revenue = SUM ('Fact Transactions'[Price]) 

Total Rides = COUNT ('Fact Transactions'[Ticket ID]) 

# Project Insights
## Total Rides by Departure Station
•	Manchester Piccadilly had the highest number of rides (~509K), followed by Liverpool Lime Street (~328K).
•	Smaller stations such as Reading and York had significantly fewer rides.
## Delayed Trips Analysis
•	Weather was the leading cause of train delays, followed by signal failures and technical issues.
•	Staffing shortages and traffic were minor contributors.
## Ticket Sales Distribution
•	90.47% of tickets sold were standard class, while only 9.53% were first class.
•	Indicates a preference for affordability over premium services.
## Revenue Trends
•	Revenue fluctuates significantly, with notable drops in March 2024, potentially due to seasonal factors.
•	Peaks observed in February and April 2024, aligning with holidays or promotional periods.

# Dashboard 
![Executive Dashboard](https://github.com/user-attachments/assets/e18629f4-fbbe-4143-ab90-5c51a00623ad)

# Final Conclusion
•	Manchester Piccadilly and Liverpool Lime Street are key hubs; optimizing these stations' services could enhance efficiency.

•	Weather-related delays suggest the need for better infrastructure to withstand harsh conditions.

•	The dominance of standard tickets indicates a price-sensitive market; premium ticket offerings might require additional perks to attract customers.

•	Revenue fluctuations highlight the importance of strategic pricing and promotions to maintain consistent income.

