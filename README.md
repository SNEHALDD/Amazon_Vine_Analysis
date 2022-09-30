# Amazon_Vine_Analysis

## Overview of the analysis
This project is about analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
From multiple datasets from "https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt", I chose "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Wireless_v1_00.tsv.gz". PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Additionally, this project contains the use of PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in this dataset.

- Deliverable 1: Perform ETL on Amazon Product Reviews
- Deliverable 2: Determine Bias of Vine Reviews
- Deliverable 3: A Written Report on the Analysis (README.md)


## Results

1) How many Vine reviews and non-Vine reviews were there?
- Vine Reviews: 
<img width="501" alt="Vine Reviews" src="https://user-images.githubusercontent.com/106944351/193182192-bcf52699-9a2b-46bf-bc41-f2016c591333.png">


- non-Vine reviews: 
<img width="505" alt="non-Vine reviews" src="https://user-images.githubusercontent.com/106944351/193182211-29319467-9699-4cee-83b8-550fb45463c2.png">


2) How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Vine 5 stars reviews: 
<img width="746" alt="Vine 5 stars reviews" src="https://user-images.githubusercontent.com/106944351/193182238-f124399d-11a1-4b95-9158-e1bbf2cbad23.png">


- Non-Vine 5 stars reviews: 
<img width="803" alt="Non-Vine 5 stars reviews" src="https://user-images.githubusercontent.com/106944351/193182266-76cf8e22-609a-43dc-a80e-042ed9be2624.png">


3) What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- 5 Stars Vine reviews Percentage: 
<img width="684" alt="5 Stars Vine reviews Percentage" src="https://user-images.githubusercontent.com/106944351/193182293-2f885e37-2875-488a-ad54-7f806925483e.png">


- 5 Stars Non-Vine reviews Percentage: 
<img width="725" alt="5 Stars Non-Vine reviews Percentage" src="https://user-images.githubusercontent.com/106944351/193182312-ff8d76b2-3a80-4b84-a63f-56f8cd14853f.png">


## Summary
1) In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement.  
- There is no positivity bias in above analysis. We can see, 5 Stars Vine reviews percentage is 36.21% and 5 Stars Non-Vine reviews percentage is 47.01%. 

2) Provide one additional analysis that you could do with the dataset to support your statement.
- It would be useful to compare the mean, median to the mean, median of the population of all beauty reviews (or even amazon reviews) to determine if the conclusion found in from this dataset can be reproduced.


