# Amazon Vine Analysis

## Overview of the Analysis

The purpose of this analysis was to analyze the relationship between review outcomes for a particular product category and whether the review was written by a member of the paid Amazon Prime program. 

In my analysis specifically, I analyzed the data for Pet Products. First, using PySpark, I performed the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance and load the transformed data into pdAdmin. Next I used PySpark to determine if there is any bias toward favorable reviews from vine members in the Pet Products Dataset. 

## Results

_How many Vine reviews and non-Vine reviews were there?_

<img align="left" src="https://github.com/hollyouellette/Amazon_Vine_Analysis/blob/main/analysis/total_reviews.png" width=200>
<br>
 In total, there were 35,768. A significant portion of these were non-Vine reviews – a total of 35,606. The remaining 162 reviews were Vine reviews.
<br><br><br><br>

_How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?_
<br>
<img align="left" src="https://github.com/hollyouellette/Amazon_Vine_Analysis/blob/main/analysis/total_5star_reviews.png" width=200>
<br>
Of the 162 vine reviews, 63 were 5 star reviews. <br>
Of the 35,606 non-vine reviews, 19444 were 5 star reviews.
<br><br><br>
_What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?_
<br>

39% of Vine reviews were 5 star reviews, while 55% of non-vine reviews were 5-star reviews.

## Summary

Based on this analysis – I would concluded that there is no positivity Bias for reviews in the Vine program for Pet Products. 

While the data skews in favour of generally more favourable ratings for non-Vine reviews – there is a significant difference in the amount of reviews for each type. With Vine reviews occupying such a low proportion of the total reviews, each review has a stronger impact on the overall percentage. 

An additional analysis that I would suggest running in this dataset is expanding the favourable review parameters to include 4 star reviews as well. While 4 is not perfect, it is still a score that would indicate the reviewer is happy with the product and would recommend it to other consumers. 

