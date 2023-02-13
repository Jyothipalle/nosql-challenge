# Module 12 Challenge - nosql-challenge
## Author : Jyothi Palle

## The challenge has three parts 
## Part 1: Database and Jupyter Notebook Set Up

* Imported the data provided in the establishments.json file from Terminal
* Load Database uk_food and the collection establishments
* Copy the text you used to import your data from your Terminal to a markdown cell in your notebook
* Import the libraries  PyMongo and Pretty Print (pprint) 
* List the databases  in MongoDB and ensure establishment present
* Assign the establishments collection for use

## Part 2: Update the database 

* Add the penang restaurent data database
* Find the business id and update in the database
* As per the request find restaurents in Dover Local authority and delete from the database
* Latitude and Longitude data stored as strings, convert to numbers with decimal

## Part 3: Exploratory Analysis
* Used analysis code for this section
* Import dependencies packages
* Create instance of mongodb client and assign establishment collections to variable from UK food database
* Analysis 1 -  Establishments with hygiene score =20 
    * count the number of records with the given criteria - 41 records
    * Display the first record from matching criteria
    * convert the matching data to data frame and print first 10 rows
* Analysis 2 -  Establishments in london having rating greter than or equal to 4  
    * count the number of records with the given criteria - 34
    * Display the first record from matching criteria
    * convert the matching data to data frame and print first 10 rows
* Analysis 3 -  Top 5 Establishments with rating of 5 and nearest to Panang resutaurent
    * Get latitude and longitude values for penang restaurent 
    * build the query within 0.01 degree either side of latitude and longitude
    * count the number of records with the given criteria - 87
    * Display the first record from matching criteria
    * convert the matching data to data frame and print top 5 records
* Analysis 4 -  Establishments in each local authority with hygiene score =0 
    * To achieve this used pipeline functionality with matching and group by criteria
    * Query the collections with aggregate function
    * count the number of records with the given criteria - 55
    * Display the first record from matching criteria
    * convert the matching data to data frame and print first 10 rows
