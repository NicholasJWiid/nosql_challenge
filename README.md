# nosql_challenge

## Project Overview
The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. The editors of a food magazine, "Eat Safe, Love" (a fictional magazine), would like to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles. The project consists of three parts: Setting up the Database, Updating the Database, and Exploratory Analysis. 

**Tools and Libraries used:**

* MongoDB
* Python: pymongo and pandas libraries
* Jupyter Notebooks

### Part 1: Database Set Up
* Import the data provided in the establishments.json file.
* Import dependencies and create an instance of the Mongo Client.
* Confirm that "uk_food" database is listed with "establishments" collection.
* Assign the establishments collection to a variable to prepare the collection for use.

### Part 2: Update the Database
* Add new restaurants to the database.
* Find BusinessTypeID for restaurant establishments and update the new restaurant with this ID.
* Remove any establishments within the Dover Local Authority from the database.
* Convert latitude and longitude to decimal numbers.
* Convert RatingValue to integer numbers.

### Part 3: Exploratory Analysis
* Count the number of documents contained in the results and display the first document.
* Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
* Write a query to return establishments that have a low hygiene score equal to 20.
* Write a query to return establishments in London that have a RatingValue greater than or equal to 4.
* Write a query to return the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added.
* Write a query to return the the establishments in each Local Authority area that have a hygiene score of 0. Sort the results from highest to lowest, and print out the top ten local authority areas.

### References
[UK Food Standards Agency (2022)](https://www.food.gov.uk/). [UK food hygiene rating data API.](https://ratings.food.gov.uk/open-data) Contains public sector information licensed under the [Open Government Licence v3.0.](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
