# Amazon_Vine_Analysis

## Overview
Since the breakout of the COVID 19 pandemic, online shopping experienced an exponential growth, many people were forced to buy everything online, during lockdowns. That also encouraged producers and sellers to place their products online, being Amazon one of the most widely used platforms for online shopping.
In these instances, product reviews are critical for a buyer to choose a product. Amazon has a paid review program called Amazon Vine, in which people are paid to review products given to them. 
The purpose of this analysis is to determine if there is a bias among the review dataset for watches sold at amazon, between vine reviewers and regular reviewers, using AWS, S3, Google Colab Notebooks and PySpark.

## Results
There is a total of 960,872 reviews on the watches dataset.
The data was filtered in order to extract only the following parameters: review id, star rating (0 to 5), helpful votes, total votes, if it is a vine review or not and if the purchase is verified.

Then the dataset was filtered to analyse only the reviews with 20 or more votes, as reviews with a low vote count are not as significant as highly voted reviews, meaning they are more accurate or precise. The number of reviews was reduced to 9,631.

Of these filtered reviews, the data was filtered again to select only the ones with over 50% helpful votes, so the number of reviews was reduced to 8,409.

Then these reviews were grouped into vine a non-vine reviews, and the number of 5 star reviews and percentage of 5 star reviews was compared between the groups, with the following findings:

 - Number of Vine reviews: 47
 - Number of 5-star Vine reviews: 5
 - Percentage of 5-star Vine reviews: 32%
 - Number of non-Vine reviews: 8362
 - Number of 5-star non-Vine reviews: 4332
 - Percentage of 5-star Vine reviews: 52%

## Summary
With this findings, we can determine that there is not a positive bias in the Vine program reviews, as the number of paid reviews is very low, and the percentage of 5-star reviews is significantly lower in the Vine program than in regular shopper reviews.
