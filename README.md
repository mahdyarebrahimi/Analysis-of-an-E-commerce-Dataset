# E-commerce Dataset Analysis

This repository contains the analysis of an e-commerce dataset. The dataset includes various user interactions with products, such as ratings, reviews, and helpfulness scores.

## Dataset

The dataset provided includes combined e-commerce data where each user can post ratings and reviews for purchased products. Additionally, other users can express their trust or distrust towards these ratings and reviews. The dataset contains information about user profiles, product details, and ratings.

### Dataset Structure

The dataset is stored in a CSV file named `A Combined E-commerce Dataset.csv`. The structure of the dataset is as follows:

| userId | gender | rating | review | item | category | helpfulness | timestamp | item_id | item_price | user_city |
|--------|--------|--------|--------|------|----------|-------------|-----------|---------|------------|-----------|

### Field Descriptions

- **userId**: The user's ID
- **gender**: The user's gender
- **rating**: The user's rating towards the item (on a scale of 1-5)
- **review**: The user's review towards the item
- **item**: The item's name
- **category**: The category of the item
- **helpfulness**: The average helpfulness of this rating (on a scale of 1-5)
- **timestamp**: The timestamp when the rating is created
- **item_id**: The item's ID
- **item_price**: The item's price
- **user_city**: The city of the user's birth

## Analysis Tasks

The analysis focuses on exploring the data and answering the following questions:

1. **General Overview**
   - Provide a summary of the dataset, including the total number of records and unique users.
   - Visualize the distribution of ratings.

2. **Product Category Analysis**
   - Analyze the rating distribution across different product categories.
   - Identify the highest and lowest-rated categories.

3. **Helpfulness and Rating Correlation**
   - Investigate the correlation between the helpfulness scores and the review ratings.
   - Visualize the relationship to understand trends.

4. **Outlier Detection and Removal**
   - Define outliers based on specific rules:
     - Reviews with helpfulness no more than 2.
     - Users who rate less than 7 items.
     - Items that receive less than 11 ratings.
   - Remove the corresponding records involving outlier users, reviews, and items.
   - Print the length of the data after outlier removal.

## How to Run

1. Clone the repository.
2. Ensure you have all necessary dependencies installed (e.g., pandas, matplotlib).
3. Open the Jupyter notebook and follow the steps outlined to complete the analysis.

## Repository Structure

- `data/` : Contains the dataset used for analysis
- `notebooks/` : Jupyter notebooks with the analysis steps
- `README.md` : This file

## Conclusion

This project demonstrates the process of analyzing an e-commerce dataset to extract insights about user behavior, product ratings, and review helpfulness. The analysis involves data exploration, visualization, and outlier detection to ensure data quality.
