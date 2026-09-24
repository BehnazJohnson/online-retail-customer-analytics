# Online Retail Customer Analysis
Customer segmentation and repeat-purchase prediction using RFM, K-Means, and machine learning.

## Project Overview
This project uses two years of transaction data from a UK online store to explore how customers shop and whether they come back. I cleaned the data, looked at sales and customer trends, grouped customers by shopping behavior, and built a model to predict who might buy again in the next 90 days.

## Main Question
Can past shopping behavior help us understand customer groups and predict who will buy again in the next 90 days?

## Dataset
I used the [Online Retail II dataset from UCI](https://archive.ics.uci.edu/dataset/502/online%2Bretail%2Bii). It has 1,067,371 rows of sales data from a UK online store, covering December 2009 to December 2011. Each row represents one product on an invoice, so one order can have several rows.

## Data Cleaning
The raw data included duplicate rows, missing customer IDs, returns, cancelled orders, and invalid prices. I removed duplicate rows and kept purchases with a customer ID, a positive quantity, and a positive price. I kept returns and cancellations separate because this analysis focuses on customer purchases.
After cleaning, 779,425 of the original 1,067,371 rows remained as valid purchases. About 22.8% of the raw rows had no customer ID, so they could not be used to study individual customers.
