# NoSQL Challenge - UK Food Hygiene Data

## Overview

The objective of this challenge was to set up a MongoDB database, perform updates on the data, and conduct an exploratory analysis of UK food hygiene ratings. The main tasks involved importing data, updating documents, and querying the database to answer specific questions about establishments and their hygiene ratings.

The project consists of two parts:

### Part 1: Database and Jupyter Notebook Setup
- Set up the MongoDB database and imported the data.
- Verified the database setup by listing databases and collections, and querying a single document.

### Part 2: Update the Database
- Added a new halal restaurant (Penang Flavours) to the collection.
- Found and updated the `BusinessTypeID` for the restaurant.
- Removed establishments located in Dover.
- Converted certain fields (latitude, longitude, and rating) to the correct data type.

### Part 3: Exploratory Analysis
Performed the following queries and analyses:
- Found establishments with a hygiene score of 20.
- Found establishments in London with a rating value greater than or equal to 4.
- Found the top 5 establishments with a rating value of 5, sorted by the lowest hygiene score, nearest to Penang Flavours.
- Analyzed how many establishments in each Local Authority area have a hygiene score of 0, sorted from highest to lowest.

## Code Explanation

- **Resources/establishments.json**: The data source file.
- **NoSQL_setup_starter.ipynb**: This notebook sets up the database and performs the initial data insertions and updates.
- **NoSQL_analysis_starter.ipynb**: This notebook contains the exploratory analysis, including queries to answer specific questions about hygiene scores, ratings, and geographical proximity.
