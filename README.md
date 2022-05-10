#                                                               Amazon Vine Analysis
 
## Overview of the analysis
In this project, we’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. We picked amazon_reviews_us_Toys_v1_00.tsv.gz to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We use PySpark to determine if there is any bias toward favorable reviews from Vine members in your dataset. 

## Results

### How many Vine reviews and non-Vine reviews were there?

![Vine reviews and non-Vine](https://user-images.githubusercontent.com/96633294/167229321-42ad0868-8afa-4939-9d67-eae2afd1dd94.png)

From a total of 63249 reviews only 29583 were vine reviews and the remaining 33711 were a non-vine reviews

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![percentage_ count_five_stars](https://user-images.githubusercontent.com/96633294/167477302-6255c3c5-817e-481d-ab31-542f2e673cf2.png)

- There are 14324 5 stars reviews in vine program. 
- There are 16090 5 stars reviews in not vine program. 

### Summary

As we can see, there is a positive bias between the vine program and the non-vine program.
It is important to note that the sample size is a bit large, but both the vine program sample and the non-vine program sample are similar.

We could improve the analysis if we filter the purchase percentage with the verified purchase column to confirm the positive bias.
