# FIFA World Cup Countries Stats [21ST CENTURY] 
## by BEKO
**Date last Updated: 15th Sept. 2023**
![FIFA](https://assets.architecturaldigest.in/photos/60082342345ead69c9c1aeb6/16:9/w_1920,c_limit/FIFA-2018-World-Cup-Featured-1366x768.jpg)

## SUMMARY OF PROJECT
This is my very first project in Data Analysis and being a huge football fan, I decided to start with the simplest datasets I found on **[Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/fifa-football-world-cup-dataset)** website, which contains all previous editions from 1930 to 2022. I went ahead with analyzing football in 21st Century (2002 -2022) because the game has vastly changed and these are the ones I experienced more. I started working with the datasets in Microsoft Excel before importing it into PostgreSQL and visualizing it with Tableau. Some stats that you will see me analyze and visualize are Games Played, Points, Wins,Draws,Losses and Win Rate.

`Part I - FIFA WC Insights.csv` - To begin with the cleaning process, some steps I took were adding and dropping columns and dealing with null values. Also, the countries column needed cleaning with duplicates such as United States and USA in the original datasets. These were all done in Excel after which I merged datasets I needed (2002-2022) from different workbooks into one simple worksheet. 

`Part II - FIFA_WC.sql` - Continuing with data validation. I created a table for validation and imported all Excel CSV data into my relational database system (PostgreSQL). I also wrote queries which determined most of the countries' statistics in the tournaments from 2002-2022. Queries like 'Countries with most: Appearances, Goals, Games played, Points won' and more. 

`Part III - Data Explore` - With this folder, you will find my analysis and visualizations of the stats. I started off by analyzing the most common stats with Postgres queries. Prior to that, I started visulizing with Pivot Tables in Excel and making a temporary dashboard before concluding visualizations in Tableau.

# 1 - Pivot Tables, Charts and Dashboard
## MS Excel Analysis
Data was organized with datasets from 2002 to 2022. My initial analysis were as follows:

`1` - In 2006, I realized Serbia and Montenegro participated as one country after which they separated into 2 independent countries ever since.

`2` - Most cells had United States while some had USA which called for data duplication. I replaced the former with the latter in my analysis.

`3` - Top 5 performing countries had the most points, best offensive records and games played in the 21st century. They are Brazil, France, Argentina, Spain and Netherlands. All countries having won the trophy except Netherlands who came close to winning it in 2010.

## Pivot Table
Pivot tables helped me to summarize my datasets by grouping and summing the data fields(Games Played, Points and Wins)

![Pivot Table](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/MS_Excel/Pivot_Table.png?raw=true)

## Pivot Charts
These charts were auto-generated from the Pivot tables and how various pivot fields were grouped. Countries and World Cup years were placed into the Filter field in the process.
![Chart1](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/MS_Excel/PivotChart1.png?raw=true)
![Chart2](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/MS_Excel/PivotChart2.png?raw=true)

## Excel Dashboard
![Excel](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/MS_Excel/Dashboard.png?raw=true)

# 2 - Stats exported from PostgreSQL
The most common statistics from the various tournaments were queried from SQL and the results were exported. The queried statistics showed the perfomance of the numerous participating countries and the difficulty of all 6 editions of the tournament.
## Data Imported Into SQL from Excel
![data](https://github.com/beko50/Portfolio/edit/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/1-Data%20import%20from%20excel.csv)
## BEST offense_Goals scored per Game
![offense](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Best%20offense_Goals%20scored%20per%20Game.csv)
## Countries with BEST Win Percentages
![win%](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Best%20win%20percentages.csv)
## Countries Wins, Draws and Losses
![WDL](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Countries%20Wins%2C%20Draws%20and%20Losses.csv)
## MOST goals scored in 21st Century
![goals](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Most%20goals%20scored%2021st%20Century.csv)
## Countries with MOST points accumulated
![points](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Most%20points%20accumulated.csv)
## Number of appearances
![apps](https://github.com/beko50/Portfolio/blob/main/Proj%231%20-%20FIFA%20World%20Cup%20Insights/Data%20Explore/PostgreSQL/Number%20of%20appearances.csv)
