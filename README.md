# Cyclistic-Project
Case study: How does a bike-share navigate speedy success?
The goal of the project is to answer the question "How do annual members and casual riders use Cyclistic bikes differently?" which would guide in creating a marketing program that would bring in more annual members registrations.

This project would be done in 3 phases; data cleaning, data exploration and analysis, and presentation of findings. 

# Phase 1: Data Cleaning
Data is the cornerstone of modern decision-making but is often messy and inconsistent. That's where data cleaning comes in. 

What is Data Cleaning?
Data cleaning, also known as data cleansing or data scrubbing, is the process of identifying and correcting errors, inconsistencies, and inaccuracies in datasets to improve their quality and reliability. It involves several steps, each aimed at ensuring that the data is accurate, complete, and formatted correctly for analysis. 

* Step 1: Importing Libraries -
  
The first step in this data-cleaning process was to import the necessary libraries. In this case, I used Pandas, a powerful data manipulation library in Python.

* Step 2: Reading the CSV Files
Next, the CSV files containing our data were read. There were a total of 13 files covering the period from January 2023 to January 2024. After reading each file as a dataframe, I used the pd.concat() function to combine each of them into a single dataframe.

* Step 3: Examining the Dataframe Structure
To get an overview of the combined dataframe's structure, I used the .info() method. This provides information about the column names, data types, and presence of missing values.

* Step 4: Dropping Columns
Sometimes, not all columns are relevant to our analysis. In this case, about 7 columns were dropped from the dataframe after thorough consideration.

* Step 5: Handling Missing Values
Missing values can adversely affect analysis. I identified 4 columns with missing values, took the count of the total number of missing values per column, and dropped rows containing missing values.

* Step 6: Standardizing the Columns
To make the dataframe more manageable, I standardized column names  by renaming those that needed to be changed to make the content clear and then converted the data types of certain columns, specifically converting float64 to datetime.

* Step 7: Checking for Duplicates
Duplicates can skew analysis results. I checked for duplicates using the .duplicated() method and I found none.

* Step 8: Saving the Cleaned Dataframe
Finally, saved the cleaned dataframe as a CSV file for future use.
