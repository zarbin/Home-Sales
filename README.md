# Home Sales - Homework 22
UTA DataViz Bootcamp <br>
04/05/2023

# Summary

In this challenge, we were asked to use our knowledge of SparkSQL to determine key metrics about home sales data. Then we used Spark to create temporary views, partition the data with parquet, cache and uncache a temporary table, and verify that the table had been uncached.

# Work and Findings

**Data Preview**

![image](https://user-images.githubusercontent.com/36682023/229989636-706db9a4-b756-49e9-af37-33be87770cb6.png)

![image](https://user-images.githubusercontent.com/36682023/229989689-8822c14b-8138-44a8-8120-f2ee85987132.png)

What is the average price for a four-bedroom house sold for each year? 

![image](https://user-images.githubusercontent.com/36682023/229991237-be3c914c-4bdb-4a8e-876f-0a6cb820c480.png)

What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? 

![image](https://user-images.githubusercontent.com/36682023/229991256-725c70b7-afea-48ad-b69a-ac77dcfede85.png)

What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?

![image](https://user-images.githubusercontent.com/36682023/229992372-7e2340eb-5385-4661-a09d-dfc0b519c464.png)

What is the "view" rating for the average price of a home where the homes are greater than # or equal to $350,000? 

![image](https://user-images.githubusercontent.com/36682023/229992724-2783d322-aad3-4151-b58d-2f7a8fe57e65.png)

Using the cached data, run the query that filters out the view ratings with average price of greater than $350,000. 

![image](https://user-images.githubusercontent.com/36682023/229992782-cc230fe5-bf64-4160-b038-2d1f58bb8e86.png)

Run the query that filters out the view ratings with average price of greater than $350,000 with the parquet DataFrame. 

![image](https://user-images.githubusercontent.com/36682023/229992824-8fde488b-1b75-4c27-b48f-086b89b610fb.png)

# Conclusion

I completed this challenge on Google Colab.  I was a bit surprised the parquet DataFrame was slower but perhaps it has to do with this being a small dataset and I imagine parquet doing better on large datasets with more fields.  The SQL was relatively straightforward and the chaching did improve runtime from 1.77 seconds to .73 seconds. 
