This repository contains two projects:  

## 1. Supervised ML - Predicting Airbnb Prices 

Project goal: Use machine learning to create a tool that can suggest a listing price for new Airbnb hosts based on the prices and characteristics of other listings in their market. 

Dataset: Bozeman, Montana, US; 10 August, 2023; downloaded from Inside Airbnb @ https://insideairbnb.com/get-the-data/


Files in this repo:

1 Airbnb Exploratory Analysis and Data Viz.ipynb : This is a streamlined, "production-ready" code file containing my exploratory analysis and data visualization code. 

2 Airbnb ML Price Predictions.ipynb : This is a streamlined, "production-ready" code file that uses supervised machine learning to predict listing price using features that would be available to a new hosts. 

3 Airbnb Full Project (Raw Code).ipynb : This is the raw code file I wrote to complete this project while familiarizing myself with the data, so it contains many data visualizations, statistics, and print statements that allowed me to better understand the data. I've included this to demonstrate how I go about understanding the data while working. 


Project steps: 

1. Data cleaning: Extracting numeric features from strings, subsetting dataset to target listings (non-institutional host, non-luxury), dealing appropriately with missing values. 
2. Feature engineering: Using my domain knowledge and insights from exploratory analysis to extract important amenities, create sensible listing types (house, apt, guest house, private room), and interact these listing types with key characteristics that predict price.
3. Exploratory Analysis: Visualizing correlations between features, analyzing geographic patterns, and visualizing property characteristics such as number of bedrooms and number of listings per host.
4. Set up pipelines to tune and train regularized regression (Lasso, Ridge, Elastic Net) and tree ensemble (Random Forest, Gradient Boosting Regressor, XGBoost Regressor) algorithms with embedded feature selection.
5. Train models, calculate performance metrics, & choose the best model. 


Results: The best model is able to predict the price with a mean absolute error of $53 and an R^2 suggesting that it captures 70% of the variation in the data.



## 2. Analysis of Bozeman's Recent Short-Term Rental (STR) Law

Project goal: Explore the effects of Bozeman's December 2023 short-term rental (STR) law on Airbnb listings. 

Background: Bozeman's December 2023 STR law banned new whole-property short-term rentals, limited where STRs could locate in the city, and (essentially) put a limit on the number of listings a host can have in Bozeman.

Data: Bozeman, Montana, US; August, 2023 - June, 2024; downloaded from Inside Airbnb @ https://insideairbnb.com/get-the-data/

Project steps in this notebook:
1. Data cleaning 
2. Classification of properties according to Bozeman's targeted STR law
3. Exploratory analysis

Results:

This preliminary analysis suggests that Bozeman's 2023 STR law reduced the total number of Airbnb listings in Bozeman by 7%, reduced the total number of active Airbnb listings by 12%, and reduced the total number of active STR Airbnb listings by 21% between August 2023 and June 2024.

I find that this decrease in the number of active STR listings is largely driven by a decrease in active STR listings of houses (-14%) & apartments (-10%), which are the most numerous listing types in Bozeman and the kinds of listings at which Bozeman's law is most targeted.

However, my results also highlight that, in the short term, roughly half of the observed decrease in STRs in Bozeman has occurred as the result of a reshuffling of properties from "short-term rental" listings (accepting stays less than 28 days) to "medium-term rental" listings (only accepting stays 28+ days), but still essentially functioning outside of Bozeman's long-term rental and housing market. 
