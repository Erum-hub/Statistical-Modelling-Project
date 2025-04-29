# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This project analyzes the geospatial distribution of New York City (NYC) bike stations and nearby Points of Interest(POIs) using data from Yelp and Foursquare. The objective is to explore how proximity to bike stations influences POI ratings from these platforms. By leveraging exploratory data analysis (EDA) and regression modeling, meaningful insights are derived about spatial clustering, user preferences, and the relationship between distance and ratings across two major review datasets.
    
## Process
### Step1: Data set preparation:
Bike station Data:
contains Latitude, longitude and details of bik stations in NYC.
    
Yelp Data:
Considered Yelp data as it provided more coverage as it Includes POI names, categories, ratings, review counts and distance from bike stations
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

    

## Results
Coefficient:
Regression Model Results
Coefficient: 0.0003, indicating a weak positive relationship between distance and Yelp ratings.

Interpretation: The impact of distance on Yelp ratings is minimal, with slight increases in ratings observed for POIs farther from bike stations.

Intercept: 4.1966.

Interpretation: Represents the baseline Yelp rating for POIs located directly next to bike stations.

Model Performance
Mean Squared Error (MSE): 0.0665, showing a relatively low prediction error.

R -squared (R²): -0.0688, indicating the model's limitations in explaining the variance in Yelp ratings based on distance alone.

## Challenges 
Understanding and combining multiple APIs required and how they work.
Deciding how to overlay different dataset and handling visualization. 

## Future Goals
Perform deeper satial analysis can be done in future.
Better use of visualization 
Utilize more techniques to learn data scraping and analysis.
