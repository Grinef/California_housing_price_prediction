# California Housing Price Prediction

## Project Overview

In this project, you will train a linear regression model using data from the California housing market in 1990. You have previously worked with this dataset in the fourth module of the course. The goal is to predict the median house value in residential blocks based on various features.

## Dataset Description

The dataset contains the following columns:

- `longitude` — Longitude.
- `latitude` — Latitude.
- `housing_median_age` — Median age of residents in the residential block.
- `total_rooms` — Total number of rooms in residential block homes.
- `total_bedrooms` — Total number of bedrooms in residential block homes.
- `population` — Number of people residing in the residential block.
- `households` — Number of households in the residential block.
- `median_income` — Median income of residents in the residential block.
- `median_house_value` — Median house value in the residential block.
- `ocean_proximity` — Proximity to the ocean.

The target variable is `median_house_value`.

## Project Steps

1. **Initialize Spark Session**: Set up a local Spark session.
2. **Load Data**: Read the dataset from `/datasets/housing.csv`.
3. **Data Exploration**: Display the data types of the columns using pySpark methods.
4. **Data Preprocessing**:
   - Check for and handle missing values appropriately.
   - Convert the categorical column (`ocean_proximity`) using One Hot Encoding.
5. **Model Building**: Build two linear regression models using the `LinearRegression` estimator from MLlib:
   - Model 1: Using all data from the file.
   - Model 2: Using only numerical variables, excluding categorical variables.
6. **Model Evaluation**: Compare the performance of the two models using the metrics RMSE, MAE, and R2. Draw conclusions based on the comparison.

## Instructions

1. Initialize a local Spark session.
2. Read the data from `/datasets/housing.csv`.
3. Display the data types of the dataset columns.
4. Preprocess the data:
   - Investigate and fill in missing values as deemed appropriate.
   - Apply One Hot Encoding to the `ocean_proximity` column.
5. Build two linear regression models:
   - One with all features.
   - One with only numerical features.
6. Evaluate the models using RMSE, MAE, and R2 metrics. Compare the results and provide conclusions.

## Submission

Once you have completed the project, submit your work for review. The reviewer will provide feedback within 24 hours. Revise your project based on the feedback and resubmit it. You may need to make several iterations based on the reviewer's comments. The project is considered complete once all revisions are approved by the reviewer.
