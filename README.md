# Creating the Optimal Daily Fantasy Lineup: 

## Using past NBA game-logs to forcast upcoming statistics 

The goal of this data science project is to create a model to forecast NBA player statistics. Using game-logs dating back to 2016, I will try to predict the statistics of each player for an upcoming game and use the predictions to create an optimal lineup to be played in DraftKings daily fantasy.

DraftKings daily fantasy is a daily contest hosted on DraftKings.com. Participants are given a list of NBA players that will be playing that night, and a salary attached to each of those players. The goal of the contest is to choose 8 players that the participant thinks will have the highest "DraftKings score" while remaining under the $50,000 salary cap. For example, LeBron James may cost $12,000 on a given night, while Joe Schmo may only cost $3,000. Choose the lineup with the highest cumulative DraftKings score, and win money!  

## DraftKings Scoring System

![plot](./images/Screen%20Shot%202021-01-22%20at%204.17.01%20PM.png)

## Data Collection 

The data for this project came in 3 parts. First, the game log data was collected from stats.nba.com. I used Selenium to webscrape the games dating back to 2016, collecting over 100,000 game logs. Second, I needed an up to date list of the current players that would be playing that night. To get data, I webscraped from www.sportsline.com. Finally, the last part of data collection scraped from www.fantasypros.com, and collected the up to date DraftKings salaries of all the players. 


