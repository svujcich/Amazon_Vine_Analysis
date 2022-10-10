# Amazon_Vine_Analysis
## Overview
A common practice many internet shoppers use to make informed decisions about purchasing products is to look at a “reviews” section on any website. To provide credible reviews for their products, Amazon started a program called Amazon Vine. In this program, individuals who have established credibility through regularly purchasing products from amazon and leaving reviews are gifted promotional items to review. Because this is an incentivized program, it presents the possibility that individuals might rate the products better than they are in reality, introducing bias. 

In this analysis, a data set of product reviews from the “outdoor” category is analyzed to determine if incentivizing reviews produces biased results. To accomplish this task, pyspark was utilized in conjunction with Google Colabratory, to extract, transform, and load the data into tables in a relational database hosted by Amazon Wes Services using pgAdmin as a server. The table holding the vine reviews data was filtered to show just the results for products that have 20 or more reviews, with at least 50% of those reviews being rated as “helpful”, and broken down paid vs. unpaid reviews. The results are as follows: 

## Results
  -	There were 39,976 reviews
      -	There were  107 Vine reviews
      -	There were 39,869 non- vine reviews
  -	Number of 5 star reviews:
      -	56 of the vine reviews were 5 star reviews
      -	21,005 if the non-vine reviews were 5 star reviews
  -	Percentage of reviews that were 5 stars:
      -	52.34% of the vine reviews received 5 star reviews
      -	52.69% of the non-vine reviews received 5 star reviews
 
## Summary  
The results indicate that the vine reviews are not bias. First, the difference between the percentage of vine reviews that received 5 star reviews and the percentage of non-vine reviews that received 5 star reviews is less than 1%. This suggests that the results of vine reviews and non-vine reviews are similar. If there was a positivity bias, it would be reasonable to expect the percentage of 5 star vine reviews would be notably greater than the percentage of non-vine reviews. Additionally, the number of vine reviews compared to non-vine reviews makes up less than 1% of the total reviews. Since the sample size of vine reviews is so small, the amount of influence the vine reviews have is not enough to create a noticeable effect on the overall consensus of the products. 

To further investigate the claims that vine reviews do not introduce bias, another analysis that might be useful would be to repeat the same analysis for each star rating. Given the total number of reviews would remain constant, investigating the number of reviews for each star rating, and calculating the percentage of reviews per star rating for both the vine and non-vine category would provide a complete breakdown of all votes cast. If the vine results echo the results of the non- vine reviews, it would provide additional support to the claim that the vine review program does not introduce positivity bias. 

