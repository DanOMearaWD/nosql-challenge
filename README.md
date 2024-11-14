# NoSQL Challenge - UK Food Hygiene Data

## Overview

This challenge aims to set up a MongoDB database, perform updates on the data, and conduct an exploratory analysis of UK food hygiene ratings. The tasks involve importing data, updating documents, and querying the database to answer specific questions about establishments and their hygiene ratings.

## Project Components

### Part 1: Database and Jupyter Notebook Setup
- Set up the MongoDB database and import data.
- Verify the database setup by listing databases and collections, and querying a single document.

### Part 2: Update the Database
- Add a new halal restaurant (Penang Flavours) to the collection.
- Update the `BusinessTypeID` for the restaurant.
- Remove establishments located in Dover.
- Convert certain fields (latitude, longitude, and rating) to the correct data type.

### Part 3: Exploratory Analysis
Perform the following queries and analyses:
- Find establishments with a hygiene score of 20.
- Find establishments in London with a rating value greater than or equal to 4.
- Identify the top 5 establishments with a rating value of 5, sorted by the lowest hygiene score, nearest to Penang Flavours.
- Analyze how many establishments in each Local Authority area have a hygiene score of 0, sorted from highest to lowest.

## Files

- **Resources**
  - `establishments.json`: The data source file.
- **Notebooks**
  - `NoSQL_setup_starter.ipynb`: Sets up the database and performs the initial data insertions and updates.
  - `NoSQL_analysis_starter.ipynb`: Contains the exploratory analysis, including queries to answer specific questions about hygiene scores, ratings, and geographical proximity.

## Key Findings

### Establishments with a Hygiene Score of 20
- **Total Number**: A significant number of establishments have a hygiene score equal to 20.
- **Sample Document**: The first matching establishment was displayed to understand the structure and data fields.
- **Data Conversion**: The results were converted into a Pandas DataFrame, with the number of rows printed and the first 10 rows displayed.

### Establishments in London with a RatingValue ≥ 4
- **Criteria**: Focused on establishments in the London area with a high rating (4 or above).
- **Total Number**: The number of documents matching this query was provided.
- **Data Analysis**: After converting to a DataFrame, the data was filtered to ensure relevance, and the top 10 rows were presented for review.

### Top 5 Establishments Near "Penang Flavours"
- **Proximity Search**: Establishments near the coordinates of "Penang Flavours" were identified (within ±0.01 degrees latitude and longitude).
- **Conditions**: Only establishments with a RatingValue of 5 were considered, sorted by the lowest hygiene score.
- **Results**: The top 5 establishments were printed and presented in a DataFrame, revealing key insights into local competition and hygiene standards.

### Hygiene Score of 0 Across Local Authorities
- **Aggregation Analysis**: A pipeline was used to find establishments with a hygiene score of 0, grouped by Local Authority.
- **Sorting**: The results were sorted from highest to lowest by the number of establishments.
- **Insights**: The number of documents was counted, and the first 10 results were printed to show which areas had the most issues with hygiene.

## Conclusion

This analysis provides a comprehensive look at hygiene standards and the distribution of restaurant ratings across various metrics. These insights can guide further research and focus areas for improving food safety.

