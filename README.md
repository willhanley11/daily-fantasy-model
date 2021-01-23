# Creating the Optimal Daily Fantasy Lineup 

## Using past NBA game-logs to forcast upcoming games 

#### The goal of this data science project is to create a model to forecast NBA player statistics. Using game-logs dating back to 2016, I will try to predict the statistics of each player for an upcoming game and use the predictions to create an optimal lineup to be played in DraftKings daily fantasy.

#### DraftKings daily fantasy is a daily contest hosted on DraftKings.com. Participants are given a list of NBA players that will be playing that night, and a salary attached to each of those players. The goal of the contest is to choose 8 players that the participant thinks will have the highest "DraftKings score" while remaining under the $50,000 salary cap. Choose the lineup with the highest cumulative DraftKings score, and win money!  

## Scoring system for each player

![plot](./images/Screen%20Shot%202021-01-22%20at%204.17.01%20PM.png)



#### My data was collected from stats.nba.com. I webscraped the game logs dating back to 2016 with a function and was able to collect over 100,000 game logs total. These game logs will be my initial inputs into the model to predict the player's next game statistics. I also created a function that scrapes the advanced stats of the opposing team's defense (if a player is playing against a better defense, maybe they won't score as well). Further, I scraped data about the rest days of each team from the previous 3 seasons. For example, how the team did when playing in back to back nights, or how they did when they played 2 games in 3 days. Putting all this together, I will create an ARIMA model to predict individual statistics on a given night. 
