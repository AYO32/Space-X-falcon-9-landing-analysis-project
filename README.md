# Space-X-Falcon-9-Landing-Analysis-Project
This  project will ultimately predict if the Space X Falcon 9 first stage will land successfully.

# Context and Business Understanding
SpaceX launches Falcon 9 rockets at a cost of around $62m. This is considerably cheaper than other providers (which usually cost upwards of $165m), and much of the savings are because SpaceX can land, and then re-use the first stage of the rocket.

If we can make predictions on whether the first stage will land, we can determine the cost of a launch, and use this information to assess whether or not an alternate company should bid against SpaceX for a rocket launch.

This project follows these steps:
1. Data Collection
   a) Making GET requests to the SpaceX REST API
   b) Web Scraping
   
2. Data Wrangling
   a) Using the .fillna() method to remove NaN values
   b) Using the .value_counts() method to determine the following:
      b.1 Number of launches on each site
      b.2 Number and occurrence of each orbit
      b.3 Number and occurrence of mission outcome per orbit type
   c) Creating a landing outcome label that shows the following:
      c.1 0 when the booster did not land successfully
      c.2 1 when the booster did land successfully
      
3. Exploratory Data Analysis
   a) Using SQL queries to manipulate and evaluate the SpaceX dataset
   b) Using Pandas and Matplotlib to visualize relationships between variables, and determine patterns 
   
4. Interactive Visual Analytics
   a) Geospatial analytics using Folium
   b) Creating an interactive dashboard using Plotly Dash  
   
5. Predictive Analysis (Classification)
 *  a) Using Scikit-Learn to:  
    *  a.1 Pre-process (standardize) the data
    *  a.2 Split the data into training and testing data using train_test_split
    *  a.3 Train different classification models
    *  a.4 Find hyperparameters using GridSearchCV
 *  b) Plotting confusion matrices for each classification model
 *  c) Assessing the accuracy of each classification model   
   
   # Key Skills Learned/Used
  * a) Using data science methodologies to define and formulate a real-world business problem
  * b) Using data analysis and data visualisation to load a dataset, clean it, and find out interesting insights from it
  * c) Interactive dashboard development with Plotly Dash
  * d) Interactive map development using Folium
  * c) Using machine learning to build a predictive model to help a business function more efficiently
  * d) Structuring and building a data-findings report
   
   
