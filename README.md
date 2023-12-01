Retail-Analysis-Machine-Learning-Approach
This repository provides the retail analysis for customer purchase behaviour using machine learning approach Introduction Retailers need help with inventory management and interpreting customer data, which can lead to overstock or stock shortages. To mitigate these challenges, we applied a machine learning model to process and analyze customer transaction data, which aids in predicting customer needs and behaviors.

Methodology Our systematic approach encompassed the following steps: Data Preparation and Cleaning: The retail dataset was thoroughly cleansed to ensure accuracy. This involved the removal of negative quantities, which typically represent returned items, and the exclusion of entries with missing values and zero-unit prices, which could skew the analysis.

Data Analysis and Visualization: We conducted a detailed exploration of the data to detect trends and patterns, utilizing visual tools to illustrate customer purchasing behavior effectively.

Customer Segmentation: Customers were categorized using the RFM (Recency, Frequency, Monetary value) method, which segments them based on their purchasing patterns. This segmentation helps distinguish between customers based on how recently they made a purchase, how often they purchase, and how much they spend.

Model Development: We constructed machine learning models to predict future customer purchases. The data was scaled using the Standard Scaler method, and K-Means Clustering was used to create distinct customer groups.

Model Evaluation: We assessed the performance of our models using metrics such as the silhouette score to measure the quality of the customer clusters formed.

Detailed Findings RFM Segmentation: The RFM analysis placed customers into four segments, scoring them from 1 to 4. A score of 1 indicated the best purchasing behavior in terms of recency, frequency, and monetary value, while a score of 4 indicated the least favorable behavior.

Behavioral Insights: Our analysis identified that the most engaged customers are recent buyers, who purchase frequently and spend more. In contrast, customers with less frequent, sporadic, and lower-value purchases posed a concern for potential churn. Visualization and Cluster Analysis: We employed scatter and box plots to visualize the relationship between purchase frequency and expenditure. This facilitated the identification of distinct customer groups and the development of targeted marketing strategies. Hierarchical Clustering: We performed hierarchical clustering for visually representing each datapoint’s relationship. In order to compare the hierarchical clustering and k-means clustering to obtain best cluster for further analysis of churn risk. Dendrogram shows the tree-like structure for each data points and their hierarchy.

Churn Risk: Churn risk is determined based on recency of more than 30 days (i.e., If customer has been in store in last 30 days the churn risk for him will be false, but churn risk will be true if the last visit was for more than 30 days.). This will determine if the customer is likely to stay loyal or not. The reason for this approach was to determine the retention strategy for each cluster of customers.
