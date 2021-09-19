# Amazon_Vine_Analysis
# Deliverable 3

This is the Deliverable 3 of Challenge 16.
.
## Overview

There are companies that pay a small fee to Amazon and provide products to Amazon Vine members, who are required to publish a review.
This assignment involved performing an ETL on Amazon Product Reviews and then to determine if there was a bias of Vine Reviews. 
The choosen dataset was: **amazon_reviews_us_Musical_Instruments_v1_00.tsv.gz**

Here are some screenshot of the data in RDS, as seen from PGAdmin.

![One table](Screenshot%20from%202021-09-18%2000-26-58.png)

![Another table](Screenshot%20from%202021-09-18%2000-27-31.png)

To download the dataset and load it into DRS, [I used SPARK](Amazon_Reviews_ETL.ipynb). The rest of the analysis was done with Pandas.
The aim is to verify if Vine reviews has more 5 star reviews than non Vine reviews.

## Results

* How many vine reviews and non-vine reviews were there?

There were a total of 572,916 reviews and there were 14,537 reviews with users with >=50% helpful ratio.
 
 Vine reviews: 60
 Non-vine reviews: 14,477
    
* How many vine reviews were five stars? How many non-vine reviews were five stars?

  There were a total of 34 5-star vine reviews and there were a total of 82,212 non-vine 5-star reviews
  
* What percentage of vine reviews were five stars? What percentage of non-vine reviews were five stars?

  Approximately 56.67% of vine reviews were 5 stars and approximately 56.72% of non-vine reviews were five stars

## Summary

With the data studied here, I found no bias in the reviews. This analisys should be repeated with more data.
The analisys can be seen in this [Jupyter Notebook](Vine_Review_Analysis.ipynb)
