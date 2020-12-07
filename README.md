# Personal-Dataset NBA 3 Point Shooting Over the Last 5 Seasons

# Motivation
I have always been a big fan of basketball at all levels, especially in the NBA. One thing I noticed from watching games and using social media is that many say the game of basketball has changed or "in today's game," directly referring to the amount of three point shooting. Numerous NBA Game announcers I watched might comment something along the lines of how the game they are watching includes more shooting than back when they played. On social media, I will often see various users comparing past and present players claiming that a player from an older generation would not be good at all in today's game because of the role 3 point shooting plays now. After seeing both highly accredited NBA Announcers, and the average NBA fan, comment on the changes in how the game is played I wondered just how much the game has changed over time. What I originally aimed to figure out was if there was a direct correlation between the amount of 3 point shooting a team does, and the amount of games they win in a season. The question I ended up answering was how much the amount of 3 point shooting across the league has increased in just the past 5 seasons.


# Data Source
I was able to obtain all of the data used in my project from the team stats section on the ![NBA Stats Page](https://www.nba.com/stats/teams/traditional/?sort=W_PCT&dir=-1), which is officially affiliated with the NBA. The website includes essentially all of the commonly tracked basketball statistics for all 30 NBA teams for every season from now (2020) back to 1997, although I only used data from 2015-2019. After selecting the season desired, a table with the statistics for all of the teams is displayed.

# Processing Steps
There were only a few steps necessary in cleaning the data. The data was easily accessible and readable via the previously listed ![NBA Stats Page](https://www.nba.com/stats/teams/traditional/?sort=W_PCT&dir=-1). All I had to do to gather this information was select the desired season I wanted to obtain (2015-16 season to 2018-19 season), and copy and paste the entire table into an excel spreadsheet. After this, I deleted all of the columns except the ones corresponding to team name, regular season record, field goals and 3 point field goals per game, and plus minus per game. I also removed an hyperlinks that were embeded in the tables as a result of copying and pasting from the NBA website. All that was left to process the data was save the excel spreadsheets and upload them to python for further analysis.

# Visualization
![Box Plots For the Seasons 2014-15 to 2018-19](https://github.com/kianwazzu/Personal-Dataset/blob/master/all%20seasons%20boxplots.png)

This shows a boxplot for number of average 3 point attempts for the whole league in the last 5 seasons.

![Ratio of 3PA to 2PA For Seasons 2014-15 to 2018-19](https://github.com/kianwazzu/Personal-Dataset/blob/master/ratio.png)

This different set of box plots shows the ratio of 3PA to 2PA per game for the last 5 seasons to prove that the increase in the amount of 3 point shooting is not an effect of a faster paced game.


# Analysis
After cleaning the data from unwanted information, I loaded each of the 5 seasons into python and made scatterplots for each season comparing 3 Point Attempts per game to Wins, while including the league average which I had to calculate, in hopes of finding applying a linear regression model to the data, however the resulting scatterplots did not show a strong relationship. While making the scatterplots for each season individually I noticed the increase in the league average 3 Point Attempts every season. Using the league average 3 Point Attempts per game I made 5 boxplots in the same space to allow me to visually see how big the increases in 3 pointers were, and the results were pretty convincing in that the amount has increased significantly. To be exact, the league average 3PA/Game in the 2014-15 season was 22.41 and in the 2018-19 season average was 32.01.
Making sure that this increase was not just due to an increase in pace (the amount of possessions per game) as a faster pace would mean an increase in almost all stats across the board, I made and compared boxplots with the ratio of 3 point shooting to 2 point shooting, which negates inflated numbers if the pace of the game increased. These too also support that 3 point shooting has increased, not due to a faster paced game, as the league average percent of field goals attempted that were 3 pointers increased from approximately 26.79% in 2014-15 to approximately 35.88% in 2018-19.
