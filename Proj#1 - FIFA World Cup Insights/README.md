# FIFA World Cup Countries Stats [21ST CENTURY] 
## by BEKO
**Date last Updated: 15th Sept. 2023**
![FIFA](https://assets.architecturaldigest.in/photos/60082342345ead69c9c1aeb6/16:9/w_1920,c_limit/FIFA-2018-World-Cup-Featured-1366x768.jpg)

## Summary of Project
This is my very first project in Data Analysis and being a huge football fan, I decided to start with the simplest datasets I found on **[Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/fifa-football-world-cup-dataset)** website, which contains all previous editions from 1930 to 2022. I went ahead with analyzing football in 21st Century (2002 -2022) because the game has vastly changed and these are the ones I experienced more. I started working with the datasets in Microsoft Excel before importing it into PostgreSQL and visualizing it with Tableau. Some stats that you will see me analyze and visualize are Games Played, Points, Wins,Draws,Losses and Win Rate.

`Part I - FIFA WC Insights.csv` - To begin with the cleaning process, some steps I took were adding and dropping columns and dealing with null values. Also, the countries column needed cleaning with duplicates such as United States and USA in the original datasets. These were all done in Excel after which I merged datasets I needed (2002-2022) from different workbooks into one simple worksheet. 

`Part II - FIFA_WC.sql` - Continuing with data validation. I created a table for validation and imported all Excel CSV data into my relational database system (PostgreSQL). I also wrote queries which determined most of the countries' statistics in the tournaments from 2002-2022. Queries like 'Countries with most: Appearances, Goals, Games played, Points won' and more. 

`Part III - Data Explore` - With this folder, you will find my analysis and visualizations of the stats. I started off by analyzing the most common stats with Postgres queries. Prior to that, I started visulizing with Pivot Tables in Excel and making a temporary dashboard before concluding visualizations in Tableau.
