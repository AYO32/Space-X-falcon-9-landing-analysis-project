# Space-X-Falcon-9-Landing-Analysis-Project
This  project will ultimately predict if the Space X Falcon 9 first stage will land successfully.

![introduction](https://user-images.githubusercontent.com/91481737/219335101-423e2631-a5b9-4683-ba89-712619dcb83b.PNG)

# Context and Business Understanding
SpaceX launches Falcon 9 rockets at a cost of around $62m. This is considerably cheaper than other providers (which usually cost upwards of $165m), and much of the savings are because SpaceX can land, and then re-use the first stage of the rocket.

If we can make predictions on whether the first stage will land, we can determine the cost of a launch, and use this information to assess whether or not an alternate company should bid against SpaceX for a rocket launch.

This project follows these steps:
1. Data Collection
   * a) Making GET requests to the SpaceX REST API
   * b) Web Scraping
   ![image](https://user-images.githubusercontent.com/91481737/219337274-d229ae5e-e349-4b65-b3cf-fa67c269609b.png)
   
2. Data Wrangling
   * a) Using the .fillna() method to remove NaN values
   * b) Using the .value_counts() method to determine the following:
      * b.1 Number of launches on each site
      * b.2 Number and occurrence of each orbit
      * b.3 Number and occurrence of mission outcome per orbit type
 * c) Creating a landing outcome label that shows the following:
     * c.1,  0 when the booster did not land successfully
     * c.2,  1 when the booster did land successfully
    ![wrangling](https://user-images.githubusercontent.com/91481737/219338682-48cd1f58-de64-4992-a9af-577b621b4efa.PNG)
     
    ![Web scraping](https://user-images.githubusercontent.com/91481737/219339879-066a3856-e646-4bbb-a978-336ef463eef9.PNG)
      
3. Exploratory Data Analysis
   * a) Using SQL queries to manipulate and evaluate the SpaceX dataset
   * b) Using Pandas and Matplotlib to visualize relationships between variables, and determine patterns 
    ![SQL](https://user-images.githubusercontent.com/91481737/219341235-8c63745f-08f8-4d8d-8ccf-2908015c310d.PNG)
   
    ![visualization](https://user-images.githubusercontent.com/91481737/219341840-7f86f92f-2872-46ed-bddc-6c50e350195f.PNG)
   
4. Interactive Visual Analytics
   * a) Geospatial analytics using Folium
   * b) Creating an interactive dashboard using Plotly Dash  
    ![FOLIUM](https://user-images.githubusercontent.com/91481737/219344387-0959b4b2-5d4c-46d4-834b-0e2fb9a8edbe.PNG)
   
    ![PLOTLY](https://user-images.githubusercontent.com/91481737/219344768-339a9e6e-1c51-4ca6-a18d-af6530b50671.PNG)
   
5. Predictive Analysis (Classification)
 *  a) Using Scikit-Learn to:  
    *  a.1 Pre-process (standardize) the data
    *  a.2 Split the data into training and testing data using train_test_split
    *  a.3 Train different classification models
    *  a.4 Find hyperparameters using GridSearchCV
 *  b) Plotting confusion matrices for each classification model
 *  c) Assessing the accuracy of each classification model   
    ![CLASSIFICATION](https://user-images.githubusercontent.com/91481737/219346038-fe8d830c-4cd4-4dc8-b9d4-376516b7a8fc.PNG)
   
 
   
   
