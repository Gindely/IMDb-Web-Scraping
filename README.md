# IMDb-Web-Scraping
Web Scraping and EDA Project
## Table of contents
* [Introduction](#introduction)
* [Technologies](#technologies)
* [Goal](#goal)
* [Dataset](#dataset)
* [Methodology](#methodology)
* [Data Overview](#data-overview)
* [Exploratory Data Analysis](#exploratory-data-analysis)
## Introduction
Scraping the IMDb website for the Top 100 most popular TV shows today.
## Technologies
Python
## Goal
The goal for this analysis is to be able to scrape the IMDb website in order to import the Top 100 most popular TV shows today and to describe the data through visualizations. 
## Dataset
The data includes 100 observations and the following variables:
<br>
*Rank:* Position held by popularity 
<br>
*Title:* Name of TV show
<br>
*Start Year:* Year the TV show was released 
<br>
*Rating:* Star rating on a scale of 0-10 
<br>
*Number of Episodes:* Number of episodes in the Series 
<br>
*Content Rating:* Rating for suitability to target audience
![Dataview](./img/dataview.png)
## Methodology
1. *Import Data:* Inspected the IMDb website to access the html code in order to determine the location for the variables needed for analysis. A for loop was then created to insert the data into lists and then to a dataframe. Data values that were missing in the Rating and Content Rating columns were filled with ‘Not Available’ and ‘Not Rated’ respectively. <br />
## Data Overview
1. *Data Understanding and Data Cleaning:* Length of the data frame and types of the variables were determined to assure that data was imported correctly. Numeric values that were stored as object were converted to numeric. After the conversion, 2 values in the Rating column were converted to NaN. Since only 2 of 100 ratings were “missing”, the mean rating was used to fill the missing values. The group by operation was used to obtain the count of tv shows in each content rating group. <br />
![Describe](./img/describe.png)
![Groupby](./img/groupby.png) <br />
## Exploratory Data Analysis
1. *Box Plot and Distribution Plot:* 
![Viz1](./img/viz1.png) <br />
2. *Histogram and Plot:* 
![Viz2](./img/viz2.png) <br />
2. *Scatterplot:* 
![Scatterplot](./img/scatterplot.png) <br />
3. *Highest Rated TV Shows:*
![HighestRated](./img/highestrated.png) <br />
4. *Lowest Rated TV Shows:*
![LowestRated](./img/lowestrated.png) <br />
