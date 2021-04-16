# **Predicting NBA Usage Rate**

Jason Kim
April 16, 2021


## Abstract

My goal with this project was to utilize data from basketball-reference.com during seasons 2016-17 to 2018-19 to create a model to predict player usage rate.
To achieve these goals, I used BeautifulSoup for web scraping, and Python libraries, including pandas, to clean the data, as well as MatPlotLib and Seaborn to create visualizations.


## Design

In the NBA, teams seek out players who can make a tangible impact on performance.

Teams utilize players in their offensive and defensive systems based on past statistics and tendencies of the players.

Based on these player attributes and statistics, a team can decide to what extent a player should be incorporated into their gameplan.


## Data

Basketball-reference data is easy to scrape, however there can be many difficulties with web scraping itself, as some page html formats may vary.


There were several issues with the data, including some player pages being nonexistent, and older season data having slightly different html format.

I utilized data from the aggregate season data for player statistics, based on per game data, advanced stats, and player metadata from each player page.

Because of the nature of my analysis, I chose to ignore entries with nan values in the Height and Weight columns, as this indicates that the player page was not working.



## Tools & Algorithms
Python Libraries:
* BeautifulSoup - Web Scraping
* SKLearn - Data Analysis & Modeling
* Pandas & Numpy - Data manipulation & cleaning
* MatPlotLib & Seaborn - Data visualizations
* Datetime - For dates


Data Import:
* Download files from basketball-reference.com database
* Combine files into a dataframe list
* Concatenate into single dataframe

Data Cleaning & Manipulation:
* Utilize Pandas to remove redundant data
* Create dataframe within range of seasons 2016-17 to 2018-19
* Remove any NaN rows from columns 'Height' and 'Weight'.

## Communication
# Visualizations:


Pairplot of Actual Data:
![usg_rt_plot](https://github.com/Jason-HKim/NBA_Regression/blob/master/Visualizations/usg_rate_plot.png)

Heatmap of Features:
![heatmap](https://github.com/Jason-HKim/NBA_Regression/blob/master/Visualizations/heatmap.png)

Pairplot of all relationships of selected features and USG%:
![nba_pairplot](https://github.com/Jason-HKim/NBA_Regression/blob/master/Visualizations/NBA_Pairplot.png)

Actual Data Points vs Predicted:
![actuals_predicted](https://github.com/Jason-HKim/NBA_Regression/blob/master/Visualizations/ActualsxPredicted.png)

Feature Coefficients:
![features_coefficients](https://github.com/Jason-HKim/NBA_Regression/blob/master/Visualizations/Features_Coefficients.png)
