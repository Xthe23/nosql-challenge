# UK Food Standards Agency Data Analysis

## Overview
This project is a comprehensive analysis of food hygiene ratings across various establishments in the United Kingdom. Contracted by the editors of the food magazine, Eat Safe, Love, our goal is to evaluate the ratings data to assist journalists and food critics in focusing their future articles on noteworthy establishments.

## Part 1: Database and Jupyter Notebook Set Up
- **Notebook**: Use `NoSQL_setup_starter.ipynb` for this section.
- **Data Import**: Import data from `establishments.json` into MongoDB. Name the database `uk_food` and the collection `establishments`.
- **Libraries**: Import necessary libraries, including PyMongo and Pretty Print (pprint).
- **Mongo Client**: Create an instance and confirm the database and collection creation.
- **Data Preparation**: Assign the `establishments` collection to a variable for further use.

## Part 2: Update the Database
- **Notebook**: Continue with `NoSQL_setup_starter.ipynb`.
- **New Establishment**: Add a new halal restaurant, "Penang Flavours", to the database.
- **BusinessTypeID**: Find and update the `BusinessTypeID` for "Restaurant/Cafe/Canteen".
- **Data Cleaning**: Remove establishments in the Dover Local Authority and convert certain string values to numeric types.

## Part 3: Exploratory Analysis
- **Notebook**: Use `NoSQL_analysis_starter.ipynb` for this section.
- **RatingValue**: Understand that it ranges from 1-5, with non-numeric values to be treated as nulls.
- **Scores**: Note that higher scores in Hygiene, Structural, and ConfidenceInManagement indicate worse conditions.
- **Analysis Questions**:
  - Establishments with a hygiene score of 20.
  - Establishments in London with a RatingValue >= 4.
  - Top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to "Penang Flavours".
  - Number of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest.

## Data Analysis Goals
- Identify high-rated establishments for potential feature articles.
- Highlight areas with poor hygiene scores for investigative reporting.
- Explore the distribution of ratings across different regions.
