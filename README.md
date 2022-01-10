# Amazon_Vine_Analysis

## Overview

The purpose of this project is to analyze Amazon reviews written by members of the paid Amazon Vine Program a service that allows manufacturers and publishers to receive reviews of their products. We will perform an ETL on Amazon product Reviews for one of the 50 given data sets provided in AWS. We will Determine if there is any bias in the Vine Reviews. The data chosen for this task is from pyspark "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Digital_Video_Games_v1_00.tsv.gz"

## Results

The dataset was probably one of the smallest one, with only 1685 total reviews recorded in it's data set in order for us to focus on reviews we first need to began to clear our data and format it so we can run analysis on them.

.<img width="960" alt="vines_y" src="https://user-images.githubusercontent.com/90356052/148714129-51c7fa44-f657-43bc-a299-a51d89f82f49.png">
as we can see by this image when we tried to pull how many Vine reviews were present in our data set our return was zero. If our code is running correctly this shows that there are no Vine reviews in our data set and all reviews are actually Non-vine.

<img width="960" alt="final_reult-vine" src="https://user-images.githubusercontent.com/90356052/148714400-80356102-ad50-442b-8232-9b16658282d9.png">
looking at the image above off our summary reported, we see that we had a total of 1685 reviews. The total 5 star reviews was 631 and our total percentage of 5 stars is 37.45. Due to our data set not containing any Vine reviews we can safely assume the the rest of 62.55 percent left over are all non-vine reviews with a rating of less than 5 stars.

## Summary

based on our results we are unable to conclude if vine and non-vine reviews show any bias due to not having vine reviews present in out data set. To further test We will need to run the same analysis on a different data set from AWS which actually contains vine reviews. Since there is plenty of databases store in AWS perhaps running this analysis on a specific product or category might give us better insights. 
