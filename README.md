# Amazon_Vine_Analysis
## Overview of the project
Analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
## Approach
use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, use PySpark to determine if there is any bias toward favorable reviews from Vine members in the selected dataset. Then, write a summary of the analysis to submit to company stakeholders.
## Tools
Python PySpark and Pandas, AWS RDS and S3 services, SQL and pgAdmin 
## Data Source
[Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)
# Results
#### Total number of reviews 
Vine reviews and percentage of 5-star reviews 
![Screen Shot 2022-09-20 at 2 17 14 AM](https://user-images.githubusercontent.com/65901034/191181704-4fa03f12-fd00-4262-9842-e93e638be0e0.png)

non-vine reviews and percentage of 5-star reviews 
![Screen Shot 2022-09-20 at 2 20 15 AM](https://user-images.githubusercontent.com/65901034/191182062-4faedf71-8857-4195-9144-f7e005af4a6b.png)

# Summary 
57% of the reviews in the Vine program were 5 stars reviews out of 285 total reviews whereas the percentage in the non-Vine reviews is 46% out of 31545 reviews. This demonstrated that a positivity bias for reviews in the Vine program.
Additionally we could analyse one-way ANNOVA test for 5-star rating for the Vine and non-Vine reviews to see whether the percentage of difference is statistically significant or not.


    
 
