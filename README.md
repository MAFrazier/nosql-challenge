## Nosql-challenge


### Using Python code, PyMongo library interacting with the MongoDB, a NoSQL database with components.

### Background:
  ### A  UK Food Standards Agency evaluates various establishments across the United Kingdom, along with their food hygiene rating for these establishments. These ratings data are evaluated in order to help journalists and food critics decide where to focus future articles.

### Part 1: Database and Jupyter Notebook Set Up
  #### 1.	Import the data provided in the establishments.json file from Terminal. Created database uk_food with collection “establishments” 
  #### 2.	Within notebook, import the libraries you need: PyMongo and Pretty Print, and created an instance of the Mongo Client.

### Part 2: Update the Database
  #### Added an exciting new halal restaurant just opened in Greenwich, and added the following information to the database:
  #### 1.	Find the BusinessTypeID for "Restaurant/Cafe/Canteen"
  #### 2.	Update the new restaurant with the BusinessTypeID.
  #### 3.	The magazine is not interested in any establishments in Dover. Establishments within the Dover Local Authority from the database was removed. 
  #### 4.	Using update_many, the number values stored as strings, were updated. Converted latitude and longitude to decimal numbers. Converted Rating Value  to integer numbers.

### Part 3: Exploratory Analysis
   #### Rating Value refers to the overall rating decided by the Food Authority and ranges from 1-5. The higher the value, the better the rating.
   #### The scores for Hygiene, Structural, and Confidence In Management work in reverse. This means, the higher the value, the worse the establishment is in these areas.
   #### The following questions are used to explore the database while using count_documents, pprint and Pandas Dataframe:
  ####1.	Which establishments have a hygiene score equal to 20?
   #### 2.	Which establishments in London have a Rating Value greater than or equal to 4?
  #### 3.	What are the top 5 establishments with a Rating Value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
  #### 4.	How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
