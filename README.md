# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
    This project analyzes the geospatial distribution of New York City (NYC) bikestations and nearby Points of Interest (POIs) using Yelp data. Specifically, it explores how proximity to bike stations affects Yelp ratings for nearby POIs. Through exploratory data analysis (EDA) and regression modeling, insights are derived about spatial clustering and user preferences.
## Process
### Step1: Data set preparation:
    Bike station Data:
    contains Latitude, longitude and details of bik stations in NYC.
    
    Yelp Data:
    Includes POI names, categories, ratings, review counts and distance from bike stations
### Step2: Merging Datasets
    - Used latitude and longitude to merge bike station and Yelp data.
    - Outer join ensures all data points are considered.

### Step3: Visualizations
    Scatter Plot:
    - Geospatial representation of bike station locations and Yelp-rated POIs.
    -Color-Coded points based on Yelp rating using Seaborn's hue=Rating

    Regression Plot:
    -Visualizes the relationship between POI ratings and their distance from bike stations
    
### Step4: Exploratory Data Analysis
    Spatial Distribution Insights
    POIs closer to bike stations tend to have higher Yelp ratings, suggesting proximity enhances user experience

### Step5: Regression Model Development
    To predict Yelp ratings based on POI distance from bike stations.


    Data Cleaning:

    Removed rows with missing values for Distance (m) and Rating.

    Model Training:

    Used Linear Regression to train the model on POI distance data.

    Split data into 80% training and 20% testing sets.

    Model Output:

    Coefficient: Indicates the impact of distance on ratings.

    Intercept: Baseline rating at zero distance.

    Performance:

    R²: Explained variance of Yelp ratings by distance.

    MSE: Accuracy of predictions.

    Visualization
    Created a regression plot to depict trends:

    Points close to the regression line show accurate predictions.

    Highlights a negative correlation between distance and ratings.

## Results
    Coefficient:
    The coefficient obtained from the model was negative (e.g., -0.0023), which shows an inverse relationship between distance and Yelp ratings.

    Explanation: This indicates that as the distance between bike stations and POIs increases, the Yelp rating decreases slightly. POIs closer to bike stations tend to have higher ratings, suggesting a preference for nearby amenities.

    Intercept:
    Example Intercept: 4.5

    Explanation: The intercept represents the baseline Yelp rating when the distance is zero (i.e., POIs directly next to bike stations). This suggests that amenities closest to bike stations already have relatively high ratings.

## Challenges 
    Understanding and combining multiple APIs required and how they work.
    Deciding how to overlay different dataset and handling visualization. 

## Future Goals
    Perform deeper satial analysis can be done in future.
    Better use of visualization 
    Utilize more techniques to learn data scraping and analysis.
