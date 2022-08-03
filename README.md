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
 
