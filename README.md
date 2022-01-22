# Amazon_Vine_Analysis

## Overview
Amazon's Vine program is a service that allows manufacturers and publishers to receive opinions about new and pre-release items from a group of trusted reviewers. Here, we perform an analytical investigation on US Video Game ratings to determine if there is any bias from Vine reviewers due to their compensation. To determine bias, product ratings from Vine members are compared against non-Vine members to identify who awards a higher percentage of 5-star reviews (i.e. votes).

## Results

An ETL process was implemented on data obtained from an Amazon S3 source for video game reviews. Over 1.7 million were recorded in this data. This data was filtered down to 40,565 by using reviews with:
* helpful vote feedback greater than 50%
* total votes greater than 20

From these, only 94 were Vine reviews and 40,471 were non-Vine reviews. A breakdown from the data can be seen in the table below:

![Rating_Percentage](https://github.com/jp3tty/Amazon_Vine_Analysis/blob/main/Images/Rating_Percentage.PNG)

How many Vine reviews and non-Vine reviews were there?
How many Vine reviews were 5 starts? How many non-Vine reviews were 5 stars?
What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?


## Summary
State if there is any positivity bias for reviews in the program.
Provide on additional analysis that you could do with the dataset to support your statement.