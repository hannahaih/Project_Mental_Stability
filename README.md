# Project Mental Stability
An analysis of mental stability in times of uncertainty

Second group project
Visualizing Real World Data

# Team Sysiphos
*[Hannah Reber]*  
*[Lam-Tuyen Nguyen]*   
*[Ulrike Anklam]*  

*[DATA FT, Berlin & 08-2020]*

## Content
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Database](#database)
- [Workflow](#workflow)
- [Links](#links)

## Project Description

In this project, we aim to examine the mental stability of the US population, indicated by the number of reported UFO sightings, in times of crisis, which is reflected by the popularity of google search topics.

## Dataset
We collected data from two different sources:

1) The National UFO Reporting Center Online Database: http://www.nuforc.org/webreports.html

2) Seach terms/topics in Google Trends: https://trends.google.com/trends/explore?q=UFO

## Database

Our Github repository contains:
- a data folder containing all CSV files
- a notebooks folder containing all Jupyter Notebooks
- a plots folder containing screenshots

## Workflow

First, we examined the ufo dataset. After some ininital cleaning, we extracted relevant columns to examine the shapes and locations of the ufos reported. In the notebooks ufo_data_shape and ufo_spotting_states, deep cleaning is processed in order to continue the plotting in Tableau. The plots obtained in Tableau can be found in the folder BeautifulPlots.

After that, we run a linear regression for the last 15 years (found in notebook linear_regression_ufo_15years). Oviously, with many unusual peaks, the regression model cannot capture much of the variations. We get only an adjusted R^2 of 0.037, which means that only 3,7% of the variation can be explained by the model. We did another regression with the data until 2019, before Corona started (notebook Analysis_v01). Here, the adjusted R^2 is even only 0.023.

As there are many unusual peaks, we plot the 15 years on each other to identity potential patterns. Like that, could see that in most of the years, in the week around the 4th od July, extremely many ufos were spotted. In 2020, however, the pattern totally stood out with a peak in April instead.

We downloaded from GoogleTrend the popularity of big events for the year around its happening. Since 2006, the starting time of our ufo dataset, we consider the financial crisis with the Obama election, Arab spring, Boston marathon bombing, Kremlin, Trump election and Coronavirus as big events which might involve lots of emotions and anxiety for the US population. We therefore plot those terms/topics in relation to the ufo data, each for its respective timeframe.

We furthered our analysis by running various statistical tests, such as seasonal decomposition, checking for autocorrelation, stationarity and we made use of the AR and ARMA model.

## Links

[Repository](https://github.com/hannahaih/Project_Mental_Stability)  
[UFO dataset](http://www.nuforc.org/webreports.html)
[Google trends](https://trends.google.com/trends/explore?q=UFO)
[Ironhack assignment](https://github.com/ironhack-datalabs/data-ber-08-20/tree/master/Projects/module-2_projects/04_visualizing-real-world-data-project)
