# NoSQL Challenge - UK Food Hygiene Data

## Overview

This challenge involves setting up a MongoDB database, performing updates on the data, and conducting an exploratory analysis of UK food hygiene ratings. The tasks include importing data, updating documents, and querying the database to gather insights about establishments and their hygiene ratings.

## Project Components

### Part 1: Database and Jupyter Notebook Setup
- Set up the MongoDB database and import data.
- Verify the setup by listing databases and collections, and querying a single document.

### Part 2: Database Updates
- Add a new halal restaurant (Penang Flavours) to the collection.
- Update the `BusinessTypeID` for the restaurant.
- Remove establishments located in Dover.
- Convert certain fields (latitude, longitude, and rating) to the correct data type.

### Part 3: Exploratory Analysis
Conduct the following queries and analyses:
- Identify establishments with a hygiene score of 20.
- Find establishments in London with a rating value of 4 or higher.
- Determine the top 5 establishments with a rating of 5, sorted by the lowest hygiene score, near Penang Flavours.
- Analyze the number of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest.

## Files

- **Resources**
  - `establishments.json`: Data source file.
- **Notebooks**
  - `NoSQL_setup_starter.ipynb`: Sets up the database and performs initial data insertions and updates.
  - `NoSQL_analysis_starter.ipynb`: Contains the exploratory analysis and specific queries about hygiene scores, ratings, and geographical proximity.

## Key Insights

### Establishments with a Hygiene Score of 20
- **Total Number**: There are several establishments with a hygiene score of 20.
- **Data Preview**: The first matching establishment's structure and data fields were reviewed.
- **Conversion**: The results were converted into a DataFrame, with the number of rows and the first 10 rows displayed.

### Establishments in London with a RatingValue ≥ 4
- **Criteria**: Focus on establishments in London with a rating of 4 or above.
- **Total Number**: The count of documents meeting this criterion.
- **Review**: Data was converted to a DataFrame, and the top 10 rows were reviewed for relevance.

### Top 5 Establishments Near "Penang Flavours"
- **Search Radius**: Establishments within ±0.01 degrees latitude and longitude of "Penang Flavours" were identified.
- **Criteria**: Only establishments with a rating of 5, sorted by the lowest hygiene score.
- **Results**: The top 5 establishments were listed in a DataFrame to reveal local competition and hygiene standards.

### Hygiene Score of 0 Across Local Authorities
- **Analysis**: Used a pipeline to find establishments with a hygiene score of 0, grouped by Local Authority.
- **Sorting**: Results were sorted by the number of establishments, from highest to lowest.
- **Review**: The top 10 results were listed to highlight areas with significant hygiene issues.

## Conclusion

This analysis provides a comprehensive view of hygiene standards and the distribution of restaurant ratings across various metrics. These insights can guide further research and focus areas for improving food safety.
