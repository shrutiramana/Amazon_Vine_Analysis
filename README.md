# Amazon_Vine_Analysis

Big Data analysis using Google Colab, Pyspark, Postgres/pgAdmin, AWS RDS, Pandas.

## Overview 
The purpose of this project is to analyze Amazon reviews written by members of the "paid Amazon Vine program". The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products and determine if there are any biases between Vine members and Non-Vine member's reviews.Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We are required to pick one of these datasets for our analysis.
To perform the analysis we - 
 1. Use PySpark to perform the ETL process to extract the dataset, transform the data,
 2. Connect to an AWS RDS instance,
 3. Load the transformed data into pgAdmin. 
 
 Next, we use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in our dataset.
 
 ## Resources
 1. Dataset - [link](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Shoes_v1_00.tsv.gz)
 2. Software - Google Colab, Spark 3.2.2, AWS RDS, postgreSQL, pgAdmin ,Jupyter Notebooks, pandas.
 
 ## Results
 
 The Dataset which was selected had about 4.3 M records. To focus on the reviews we filter the dataset by following - 

 
![Screen Shot 2022-08-03 at 5 20 57 PM](https://user-images.githubusercontent.com/98556229/182722531-23ffdfa5-5896-4674-b944-06d001b441f8.png)

 - with Total votes equal to or greater than 20. This fetched 27884 records.
 ![Screen Shot 2022-08-03 at 5 24 43 PM](https://user-images.githubusercontent.com/98556229/182722884-0169a41b-d879-427d-9377-09770793ad50.png)

 - with percent of (Helpful_votes /Total_votes) greater than or equal to 50%. This fetched 27009 records , reducing the number of records for analysis.
 ![image](https://user-images.githubusercontent.com/98556229/182723045-8b934f3b-d631-4b02-8683-12cfe6e90656.png)
 
- How many Vine reviews and non-Vine reviews were there?
Total Vine Review - 22 
Total Non-Vine reviews - 26987


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
Total 5-star Vine reviews - 13
Total 5-star Non-Vine reviews - 14475

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

The percentage of vine reviews - 59.09%
The percentage of non Vine reviews - 53.63%

Below screen shows the same for the dataset.
![Screen Shot 2022-08-03 at 5 29 41 PM](https://user-images.githubusercontent.com/98556229/182723434-4d48f654-0184-4403-bf7c-aa6144d07b5d.png)

