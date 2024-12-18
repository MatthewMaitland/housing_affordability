# Nashville Housing

## Canva Slides presentation
Link: https://www.canva.com/design/DAGZIsvVhfc/vpw26cU-PqrIURXusm_Htw/edit

## PowerBI Dashboard
Link:https://app.powerbi.com/groups/me/reports/678b08c5-5801-4070-9670-3569de88fd15/c9a626839be773cc4570?experience=power-bi

## Table of Contents
* [PowerBI](#Tableau-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data](#normaling-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Sources](#sources)
* [Conclusion](#conclusion)

## Motivation:
As my friends and I were sitting around discussing our housing situations, some just bought a house with a mortgage payment of over $3000.  Another couple just sold their house and are currently renting because they could not find another home they could afford.  And then there is me.  A single father who also takes care of his mother and niece, who currently rents, and has less than $20,000 in savings.  Currently the situation looks bleak for finding an affordable home to own.  So, I wanted to do some analysis around this unattainable portion of the American Dream.


## Questions:
1) Can the average Davidson County resident afford a home large enough for the average size family?
2) How much do they have to sacrifice quality of life and safety to do so?
3) What other factors affect the cost of housing?
4) What are the differences between the areas with the highest cost homes and lowest cost homes?
5) What would be the best area to purchase a home when considering all these factors?
6) How long would it take to save enough money to purchase said home, and how long would it take to pay it off?  (And we'll compare this across a wide range of income levels)


## Normalizing the Data
I obtained information nashvillesmls.com, niche.com, and a survey of Davidson County residents as well as crime statistics from data.nashville.gov. I took the data from the survey which ranged from Very Dissatisfied to Very Satisfied and created a loop in Python to assign numeric values to each choice. I then created heatmapts across a wide variety of topics using Davidson County zip codes in geospatial; plotting major cities on them for points of reference. Finally I merged all my tables into one full_table for ease of comparison.


## Problems and Hurdles
My largest hurdle was finding data about a subject I was passionate about.  Fortunately being able to afford a home in a nice area is something nearly everyone is passionate about.  I also had issues working with the chloropleth measurement bars on the right of the map, and it took a fair amount of trial and error to work with them.  Also, in order to drop the blank entries in the surveys where someone skipped a question, I had to break the survey down into a separate table for each question before re-merging all of them into a single dataframe.


## Technologies Used
1) Python / Pandas - for exploration, normalizing and aggregation of the dataset
2) PowerBI - for creating interactive dashboard
3) Canva - for introduction of Project


## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

1) nashvillesmls.com for information about housing hosts in each zip code as well as a cost of living guide
https://www.nashvillesmls.com/nashville-area-zip-codes/37221-real-estate.php
https://www.nashvillesmls.com/blog/cost-of-living-in-nashville.html

2) niche.com provided information on how users rated each zip code as well as their public schools; it also provided the population for each county
https://www.niche.com/places-to-live/search/best-zip-codes-to-live/m/nashville-metro-area/?page=1

3) nerdwallet.com provided an example calculator for determining housing costs and interest rates
https://www.nerdwallet.com/mortgages/mortgage-calculator/tennessee

6) data.nashville.gov provided data on how metro residents feel about things by zip code, government employee salaries, and crime stats by zip code
Survey:
https://data.nashville.gov/datasets/74fb39eed1e1457f8459e8101962adf1_0/explore
Salaries:
https://data.nashville.gov/datasets/8a9e12d4ab7045b8a6cc26c0f93e1c50_0/explore
Crime:
https://data.nashville.gov/datasets/d747436243e9439e968fce056545016a_0/explore?location=35.878884%2C-86.948355%2C7.40

## Conclusion
Housing prices are at an all time high in America and specifically here in Nashville.  However, the minimum wage has not changed from $7.25 since it was set there in 2009.  Given the lack of a correlated increase in wages over the last 15 years, there is a very small window for a single person to be able to afford a home.  Even if that person is working for the very city in which they are trying to live.