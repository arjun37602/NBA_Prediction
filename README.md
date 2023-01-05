Personal Project - NBA Data Analysis using machine learning, web scraping, and Python visualization

Data: Every single NBA player's stats and their likelihood of being voted as MVP from the years 1991-2021. The chance of winning MVP is measured using the 
award_share column. Value between 0 and 1 derived from voting panel. This model can predict voting panel scores for MVP candidates with a 97% accuracy rate
using player information such as 3Pt percentage, assists, blocks, steals, freethrow percentage, etc during a season. 

<img width="445" alt="image" src="https://user-images.githubusercontent.com/33012834/210685356-124b2e33-3788-4636-a145-0a688f7d3b96.png">

<img width="497" alt="image" src="https://user-images.githubusercontent.com/33012834/210685774-420622f7-243a-4be4-8a40-6ccc426ff9a3.png">
<img width="289" alt="image" src="https://user-images.githubusercontent.com/33012834/210685801-1e3a406f-7080-4b0f-a400-ba95d70f0907.png">

Various statistical tests including R^2, MSE, RMS demonstrate error rate < 4%. Strong R^2 value .97 close to 1. Graph of actual and predicted values of MVP 
voting points is very similar, with most predicted values lying on actual values line. 

#################################################

<img width="578" alt="image" src="https://user-images.githubusercontent.com/33012834/210687102-55af6ec9-bbff-419a-b8f0-999bd5e12a26.png">

Single variable linear regression. Asseses how the win percentage of a candidate's team determines their chance of winning MVP. Poor r^2 value of .15
demonstrates no correlation. Scatter plot also demonstrates points all over the place with no line of best fit. 

<img width="257" alt="image" src="https://user-images.githubusercontent.com/33012834/210687347-551e86c8-35f3-4b12-96fc-efdd99c8b1e7.png">

Rather this model allows us to infer that MVP is purely based on an individual player's performance rather than team performance. 
Graph of player's points per game and likelihoodof winning MVP shows strong positive correlation. Logistic regression model demonstrated r^2 value > 13000,
indicating it is incorrect choice of prediction. 

<img width="279" alt="image" src="https://user-images.githubusercontent.com/33012834/210687494-95acd449-8c9d-4e9c-8f74-fb14a4dabbce.png">

PART 2 of Project: Web Scraping

Scraped Golden State Warrior's page on basketballreference.com and extracted roaster stats through python's beatiful soup library. 

<img width="843" alt="image" src="https://user-images.githubusercontent.com/33012834/210687942-2834fabf-2eba-4663-9352-40bf346b4623.png">

Iteratively extracted players individual person achievements by scraping their personal websites through URL data concatenation. Derived every
warrior's player's achievement during their career. Also scraped personal demographic data such as height, weight, twitter handle, etc by iteratively
scraping. Get_stats function on index.py provides every players data from 1991-2021 when a year in inputted. 

<img width="1129" alt="image" src="https://user-images.githubusercontent.com/33012834/210688967-160182a7-ea91-440b-b6da-fe9cb21f2dd7.png">

