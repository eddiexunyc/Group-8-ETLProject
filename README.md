# Starbucks Stores vs Weather Location Analysis

Team Members: 
- Eddie Xu
- Mackenzie Baucum
- Vasudha Nair

Project Description: By using the ETL, our team is trying to determine the weather conditions that were prevalent at various Starbucks locations in the US. We will be studying the various aspects of the weather.
  - Extract: The weather data is a JSON file that is converted into a CSV file and the Starbucks data is a CSV file.
  - Transform: In order to transform the public data and use it in our study we performed the following: 
    - Used Pandas functions in Jupyter Notebook to load the CSV and the JSON file
    - Reviewed the files and transformed into data frames.
    - For the Starbucks Data set we only focused on Starbucks Brand (there were other brands as well). The data has all the locations in the world. We narrowed it down to USA.
    - Next we dropped the locations that did not have a Postcode and looked at the unique cities for these locations. 
    - For the Weather Data, we focused on cities for the Starbucks locations in the USA and queried it based on API. We filter out any KeyError errors if the city is not found.
    - Joined the two data sets by City (inner)
    - Created queries to address our question
  - Load: Load: We transfered our output into a Database. We created a database and respective table to match the columns using Postgres database (PG admin) to store our original clean data sets. We reconnected to the database and generated additional tables for the data frames. There are some limitations to our findings due to the data available. However, we were able to address our hypothesis question in our initial project proposal listed in the ETL Project Final Technical Report

Datasets:
- Open Weather Map API (http://api.openweathermap.org/data/2.5/weather?)
- Starbuck Locations Data (https://www.kaggle.com/starbucks/store-locations)

