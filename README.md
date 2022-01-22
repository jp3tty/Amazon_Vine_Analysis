# Amazon_Vine_Analysis

## Overview
Amazon's Vine program is a service that allows manufacturers and publishers to receive opinions about new and pre-release items from a group of trusted reviewers. Here, we perform an analytical investigation on US Video Game ratings to determine if there is any bias from Vine reviewers due to their compensation. To determine bias, product ratings from Vine members are compared against non-Vine members to identify who awards a higher percentage of 5-star reviews (i.e. votes).

## Results

An ETL process was implemented on data obtained from an Amazon S3 source for video game reviews. Over 1.7 million reviews were compiled in this data, which was filtered down to 40,565 by using reviews with:
* helpful vote feedback greater than 50%
* total votes greater than 20

From these, 94 were Vine reviews and 40,471 were non-Vine reviews. A breakdown from the data can be seen in the table below:

![Rating_Percentage](https://github.com/jp3tty/Amazon_Vine_Analysis/blob/main/Images/Rating_Percentage.PNG)


## Summary

Video game manufacturers and publishers appear to benefit from being a part of the Amazon Vine program. The table above shows that Vine members receive 5-star ratings 51% of the time, while non-Vine members receive 5-star ratings 38% of the time. Based on these results it's clear that there is a positivity bias with Vine memberships when it comes to product reviews. To further investigate for positivity bias the data could be grouped into percentages for each star rating.