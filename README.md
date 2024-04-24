# Customer_Personality_Analysis

## Customer Personality Analysis

Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviors, and concerns of different types of customers.

This project aims to perform clustering to summarize customer segments based on various attributes such as demographic information, purchasing behavior, and response to marketing campaigns.



## Dataset

The dataset contains information about customers, their purchases, promotions, and demographics. Attributes include:

People: ID, Year_Birth, Education, Marital_Status, Income, Kidhome, Teenhome, Dt_Customer, Recency, Complain

Products: MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds

Promotion: NumDealsPurchases, AcceptedCmp1-5, Response

Place: NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumWebVisitsMonth


## Approach

## Exploratory Data Analysis (EDA)

Cleaned missing values in the 'Income' column by filling them with the median income of the respective education level.

Converted the 'Dt_Customer' column to datetime format.

Visualized the data distribution using histograms and box plots.

Analyzed the count of customers by year of birth.


## Feature Engineering

Added new features such as 'age_at_enroll', 'days_customer_for', 'num_children', 'has_children', 'num_total_purchases', 'total_Mnt', 'accepted_any_cmp' based on existing columns.

## Data Preprocessing

Applied one-hot encoding for categorical columns ('Education', 'Marital_Status').

Scaled numerical columns using StandardScaler.

Reduced dimensionality using PCA.

## Clustering (KMeans)
Applied KMeans clustering to segment customers into distinct clusters.

Determined the optimal number of clusters using the elbow method.

Visualized clusters using PCA.


## Results and Insights
Identified four customer clusters based on spending behavior, demographics, and other attributes.

Provided recommendations for each cluster, such as targeted marketing strategies and product offerings.

## Business Insights and Recommendations
- Cluster 0: High Affluent and High Spender - Target with premium products and offers.
- Cluster 1: Middle income and Middle spender - Focus on personalized offers.
- Cluster 2: Low Income, Low Spend - Offer budget-friendly options and promotions.
- Cluster 3: Lowest Income, Low Spend - Focus on value and convenience.

  
## skills and tools 
 Python: For data cleaning, analysis, and visualization.
  
-Pandas: For data manipulation and analysis.

-NumPy: For numerical operations.

-Matplotlib and Seaborn: For data visualization.

-Scikit-learn: For machine learning tasks such as clustering.

-Google Colab: For accessing and working with the dataset.

## Conclusion
Customer Personality Analysis is crucial for businesses to tailor their products and marketing strategies to different customer segments. By understanding customer preferences and behavior, businesses can improve customer satisfaction and loyalty, ultimately leading to increased revenue and growth.
