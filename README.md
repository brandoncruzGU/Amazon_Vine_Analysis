# Amazon Vine Analysis

## Analysis Overview
This analysis uses Amazon Vine datasets to determine whether there is a bias toward favorable furniture reviews from Vine members versus non-Vine members. The first step of this analysis uses PySpark to extract the data from the Amazon datasets, transforms them using PySpark in Google Collab, and then loads them into a data base using SQL. Lastly, several Pandas functions were used to create filtered data frames to house the data for Vine and Non-Vine member reviews for the final analysis.

## Results

### Total Number of Reviews per Group
There is a total of 136 Vine Reviews and a total of 18,019 Non-vine reviews. The totals were calculated using the len function to count the length of each respective data frame.
![image](https://user-images.githubusercontent.com/107777321/201472545-5843b35f-3d55-4cd1-a66b-105ec6209da0.png)

### 5-Star Reviews by Group
Of the 136 total Vine reviews, 74 provided a 5-star rating. Of the 18,019 total Non-vine reviews, 8,482 provided a 5-star rating. These totals were calculated using the sum function that counts the rows within the star_rating column that equal 5.
![image](https://user-images.githubusercontent.com/107777321/201472722-b886beb0-9633-4065-b1a4-058d8793e9c2.png)

### Percentage of 5-Star Reviews by Group
54.4% of the Vine members gave 5-star ratings in their reviews. 47.1% of Non-vine member gave 5-star ratings in their reviews. These percentages were calculated by dividing the number of 5-star ratings and the total number of reviews for each respective group.
![image](https://user-images.githubusercontent.com/107777321/201472821-bb2d4103-8abb-433c-910e-0b9af2e8ef57.png)

## Summary
Given the small difference (approximately 7%) between the percentage of 5-star ratings of the Vine (54.4%) and Non-vine groups (47.1%), I would say that the effects of positivity bias are extremely minimal, if there are any at all. This means that the reviews for products within the furniture department are fairly similar for both Vine and Non-Vine members. 

To further test the reliability and bias of Vine member reviews, we can do an analysis of several datasets from other types of products to see how the bias may change based on the product type. 
