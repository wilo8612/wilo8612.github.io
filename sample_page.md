Final Project Report – Zomato Analysis
By William Loaiza

Executive Summary
This project analyzes restaurants performance, cuisine preferences, and User performance using Zomato data from 2017 to 2020. The goal was to support Zomato’s strategic shift to a Cloud Kitchen model, aiming to become a $100 million business by 2030. Key insights revealed that highly rated, affordable restaurants with popular cuisines such as North Indian and Chinese are ideal candidates for cloud kitchen integration. The project recommends prioritizing these restaurant types, tailoring offerings to demographic trends, and using data to optimize partnerships and menu design.

Introduction and Methodology
Zomato, a leader in food delivery and restaurant discovery, is transitioning toward a Cloud Kitchen model to scale operations and improve profitability. This project aimed to identify which restaurants and menu items should be prioritized in this transition based on performance and customer preferences.
Scope of Analysis:
Data range: 2017–2020


Focus: Restaurant performance (Revenue, Qty Orders and Rating), customer demographics, and menu popularity.
Methodology:
Data Source: 


Orders Table: Stores details like order date, time, quantity, amount, currency, user ID, and restaurant ID.



Restaurant Table: Includes restaurant details such as ID, name, location, rating, cost, cuisine, license number, and contact information.


Users Table: Stores user profiles with ID, name, email, password, age, gender, marital status, occupation, income, education, and family size.


Data Cleaning: Handled null values, removed duplicates, and corrected inconsistent formatting. All using Tableau through calculated fields and data filtering.
The Zomato dataset includes several entries with missing values in the 'Restaurant Id' column, suggesting that some orders were placed at establishments that were either unlisted or could not be identified in the data. These entries were excluded from the visualizations specifically related to restaurant performance analysis. The total sales amount associated with these unidentified restaurants is USD 264,292, representing approximately 2.30% of the dataset's overall revenue.
Data Modeling: This report uses the Orders, Restaurants, and Users tables. In Tableau, one-to-many relationships were established between the Orders and Restaurants tables using the 'Restaurant ID' column, and between the Users and Orders tables using the 'User ID' column.


Data Transformation: Separated multiple cuisine types that were stored in a single field, standardized sales amounts to a single currency (1 USD = 85.96 INR 04/08/2025), and converted text fields—such as the 'Cost' column in the Restaurant table—into numerical values to enable grouping by category.


Exploratory Analysis: Developed a series of visualizations questions and validate initial hypotheses. These visualizations included bar charts, scatter plots, line graphs, and tables.


Data Presentation, Findings, and Recommendations
Key Findings
1. Cuisine & Menu Preferences
Across all years and cities analyzed, North Indian and Chinese cuisines consistently ranked as the most popular choices among customers, indicating a strong and sustained preference for these two types of food regardless of location or time period.
Most Ordered Cuisine


Although Chinese and North Indian cuisines are the most preferred overall, internationally recognized restaurant chains such as Domino’s Pizza, Pizza Hut or KFC consistently rank among the top revenue-generating establishments.






         Top Revenue by Restaurant


Recommendation: Focus cloud kitchen offerings on high-demand cuisines and select the most revenue-generating Restaurants that offer North Indian and Chinese Cuisine.
Preferred Cuisine per City

North Indian and Chinese cuisines are the most consistently ordered across all cities, with Noida-1, Bikaner, and Indirapuram (Delhi) leading in overall volume. Indian cuisine maintains moderate popularity, while Snacks and Biryani show stronger regional appeal—particularly in Bangalore neighborhoods such as Electronic City and Indiranagar, where Biryani stands out. These trends reveal both widespread preferences and local variations, suggesting opportunities for targeted strategies and growth in niche categories.

2. Top-Performing Restaurants
While it is not possible to conclude that the restaurants with the highest number of orders are also those with the highest ratings, the data shows that restaurants with more than 500 reviews have an average rating of 3.82. Additionally, 66.43% of all rated restaurants fall within the 4-star rating bin. The following table presents the top-rated restaurants within each cuisine category. 


For instance, Domino’s Pizza holds the highest rating in the Pizza category. Interestingly, Chinese and North Indian cuisines—which are among the most ordered—are not represented among the top-rated restaurants. This contrast highlights a potential area for improvement, especially when compared to categories like Snacks, Desserts, and Beverages, which tend to receive higher customer ratings.


Higher sales amounts do not necessarily translate into lower order frequency per customer. As shown in the chart, there is no clear inverse relationship between order frequency and sales amount. 






Customers with both high and low frequency can be seen across the full range of sales amounts, indicating that larger purchases are not exclusively made by less frequent buyers. This suggests a diverse customer base with varying purchasing behaviors, where high-value orders may occur regardless of how often a customer places them.


Restaurants with lower costs received 89,68% of the total orders.

Recommendation: Partner with restaurants that have both high ratings above the average and top number of orders.

3. Customer Demographics
Among all demographic groups, students have the highest average spend per order. However, the difference in average spending across the groups is relatively small, indicating that purchasing behavior remains fairly consistent regardless of demographic category.





Conclusion and Appendices
Conclusion
Cuisine and Menu Preferences: North Indian and Chinese cuisines are the most popular across all cities and years. These should be prioritized for cloud kitchens, as they show sustained demand. Regional variations, like the popularity of Biryani in Bangalore, offer opportunities for tailored menus.


Restaurant Performance: Restaurants with higher ratings and a large number of orders perform better. There is an opportunity to improve quality in popular cuisines such as North Indian and Chinese. Cost-effective, high-rated restaurants should be prioritized for partnerships.


Customer Demographics: Students have the highest average spend per order, but overall spending behavior remains consistent across demographics. This insight can guide targeted marketing strategies, especially toward student customers.


Recommendations:


Focus on North Indian and Chinese cuisines for cloud kitchen offerings.


Partner with cost-effective, high-rated restaurants that have strong order volumes.


Leverage regional preferences like Biryani in specific cities.


Tailor marketing to target demographics, particularly students.

