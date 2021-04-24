# Amazon_Vine_Analysis

## Overview
The following report analyzes Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

This project uses the Amazon pet products dataset to evaluate bias toward favorable reviews from Vine members. 

__Tools:__ 
  * PySpark 3.1.1
  * pgAdmin 4.29 and PostgreSQL 
  * Amazon RDS (AWS Console)
  * [Amazon pet products dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz)

## Results 
How many Vine reviews and non-Vine reviews were there? 
  * There are 170 Vine reviews in the dataset, compared to 37840 unpaid reviews. 


How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  * 65 of 20677 five star reviews were made by Vine reviews. The rest of the five star reviews (20612) were made by non-Vine members.

What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  * 0.3% of the five star reviews were made by Vine reviewers. This means that 99.7% of the reviews were made by non-Vine members.
  * Of all the Vine reviews, 38.2% of them were five stars. Comparatively, for unpaid reviews, 54.5% of the total reviews were five stars. 

## Summary 

It is hard to say that there is much bias in the Vine program based on this analysis alone, as there are 170 total paid reviews in this dataset. However, if a conclusion had to be drawn from this data, it appears that participation in the Vine program does not equal better reviews. Vine reviewers tended to five five star ratings at a lower rate compared to unpaid reviewers. 
