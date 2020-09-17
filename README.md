# Project Mental Stability
An analysis of mental stability in times of global crisis 

Second group project
Visualizing Real World Data

# Team Sysiphos
*[Hannah Reber]*  
*[Lam-Tuyen Nguyen]*   
*[Ulrike Anklam]*  

*[DATA FT, Berlin & 08-2020]*

## Content
- [Project Description](#project-description)
- [Questions & Hypotheses](#questions-hypotheses)
- [Dataset](#dataset)
- [Database](#database)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description

The goal of our project was to analyse and visualize a real world datasets and identify potential correlations. The topic was chosen after collaborative research on available datasets, based on group interest and posibilities for analysis. We wanted to use data that can be applied to recent global developments of interest. 

## Questions & Hypotheses

With this project, we created a hypothesis that there is a correlation in the mental stability of a population, represented in the number of reported UFO sitings and global crisis. 

The project focuses on answering the following questions:

1) Is there a correlation between the number of UFO siting reports and global crisis?
2) Is there a correlation between the number of UFO sitings and certain search terms during the same period?
3) What does this tell us about the mental health of the US population during the Covid19 Pandemic?

## Dataset
We decided to collect and analyse data from two different sources. The datasets were collected via download as CSV files.

We used the following source for report data on UFO sitings:

1) http://www.nuforc.org/webreports.html
The National UFO Reporting Center Online Database

For the data on search terms we used Google Trends:

2) https://trends.google.com/trends/explore?q=UFO

## Database

Our Github repository contains:
- a data folder containing all CSV files
- a notebooks folder containing all Jupyter Notebooks
- a plots folder containing screenshots of a few plots generated in Tabelau for instance

## Workflow

First, we examined to ufo dataset. After some ininital cleaning, we extracted relevant columns to examine the shapes and locations of the ufos reported. In the notebooks ufo_data_shape and ufo_spotting_states, deep cleaning is processed in order to continue the plotting in Tableau. The plots obtained in Tableau can be found in the folder BeautifulPlots.

After that, we run a linear regression for the last 15 years (found in notebook linear_regression_ufo_15years). Oviously, with many unusual peaks, the regression model cannot capture much of the variations. We get only an adjusted R^2 of 3,7%. 
We did another regression with the data until 2019, before Corona started (notebook Analysis_v01). Here, the adjusted R^2 is even only 2,3%.

As there seems to be many returning peaks, we plot the 15 years over the period of its year. Like that, we could identify a similar pattern for many years: In the week of July 4th, extremely many ufos are spotted. 2 years follow a different pattern: in 2020 there was a huge peak in March, in the beginning of the crisis and in 2015, there was a peak in December.

We downloaded from GoogleTrend the popularity of events for the year arounds its happening. Since 2006, the starting time of our ufo dataset, we considers the financial crisis, Obama election, Arab spring, Boston marathon bombing, Kremlin, Trump election and Coronavirus as big events (or crisis) that involve emotions. We therefore plot those terms/topics with the ufo data, each for its respective timeframe.

From that we can see, in 2020, after the Corona pandemic occured, many more ufos were spotted. 





The workflow was outlined in Trello (link below in 'Links' section). The first step was to discuss the topic and achieve an agreement. Afterwards, we reflected individually about what we aimed for as personal development and what were our strengths and weaknesses. Then we individually researched the two data sources and explored the possibilities of analysis that the data offers. 



## Organization

We used Trello (link in 'Links' section) to organise our workflow as described in the previous section.



## Links

The links to repository, presentation slides and trello board are:

[Repository](https://github.com/Ulli-H/Project_Mental_stability)  
[Slides](https://slides.com/lam-tuyen/deck-1e0339/review)
[Trello](https://trello.com/b/C2Ff4Bz8/team-sysiphos-mental-stability-in-times-of-crisis) 
