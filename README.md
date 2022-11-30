# Big-Data-Challenge

# Overview
In this assignment, you will put your ETL skills to the test. Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. They are quite large and can exceed the capacity of local machines. One dataset alone contains over 1.5 million rows; with over 40 datasets, data analysis can be very demanding on the average local computer. Your first goal for this assignment will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

# Instructions/Level 1

Use the provided schema to create tables in your RDS database.

Create two separate Google Colab notebooks and extract any two datasets from the list at review dataset. Put each dataset into its own notebook.
Note: You could ETL both data sources in a single Colab notebook, but it will be easier to work with these large S3 data sources in separate notebooks.

Be sure to handle the header correctly. If you read the file without the header parameter, you may find that the column headers are included in the table rows.

Complete the following steps for each notebook (one dataset per notebook).

Count the number of records (rows) in the dataset.

Transform the dataset to fit the tables in the schema file. Be sure that the DataFrames match in data type and in column name.

Load the DataFrames that correspond to tables into an RDS instance. Note: This process can take up to 10 minutes for each. Ensure that everything is correct before uploading.

# Resources 

Amazon customer review dataset files: 

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz

https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz

# ETL difficulties 

I was able to perform the Extract and Transform steps of the process and connect to my PostgreSQL RDS, but the load process would not complete. The process was loading for 25+ minutes and still wouldn't work. I was also able to create the tables in my SQL database with the schema.sql file. I was able to see the "error" message on AWS when I cancelled the cell in the notebook. This tells me that the connection was there, I just missed something else along the way. 



