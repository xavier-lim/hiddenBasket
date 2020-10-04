# HiddenBasket
![HiddenBasket Header](https://github.com/xavier-lim/hiddenbasket/blob/master/images/DG.jpg)

HiddenBasket uses several statistical methods including logistic regression and discriminant analysis to do the following:
1.	Classify players into groups (tiers) based on their salary
2.	Determine the relationship/correlation between salary and various player performance statistics
3.	Determine which performance statistics significantly impact player salaries 
4.	Determine which combination of factors predict player salaries
5.	Determine the players who are predicted to be of a higher salary, i.e. undervalued

To view the article I wrote about my model on LinkedIn, please visit: [HiddenBasket: The Most Undervalued NBA Players](https://www.linkedin.com/pulse/hiddenbasket-most-undervalued-nba-players-xavier-lim-2f)

## Table of Contents
1.	[Project Tools](https://github.com/xavier-lim/hiddenbasket#project-tools)
2.	[Data Source](https://github.com/xavier-lim/hiddenbasket#data-source)
3.	[Tableau Project Dashboards](https://github.com/xavier-lim/hiddenbasket#tableau-project-dashboards)
4.	[Conclusion](https://github.com/xavier-lim/hiddenbasket#conclusion)
5.	[Acknowledgements](https://github.com/xavier-lim/hiddenbasket#acknowledgements)
6.	[Author](https://github.com/xavier-lim/hiddenbasket#author)

## Project Tools
1.	RStudio - [RStudio Desktop](https://rstudio.com/products/rstudio/download/) OR [RStudio Cloud](https://rstudio.cloud/)
2.	NBA Player Performance Statistics Data Frame Source – “GamePerformance” Sheet of nba_data.xlsx
3.	NBA Player Salaries Data Frame Source – “Salaries” Sheet of nba_data.xlsx
4.	NBA Player Efficiency Rating Data Frame Source – “EfficiencyRating” Sheet of nba_data.xlsx

## Data Source
For my project, I collected three data sets from [Basketball Reference](https://www.basketball-reference.com/):

1.	The **Player Performance Statistics** data set presents information and performance statistics about each player (*514* in total) such as their position (Pos), age (Age), team (Tm), games played (G), rebounds per game (REB), assists per game (AST), blocks per game (BLK), and points per game (PTS).
2.	The **Player Efficiency Rating** data set presents the player efficiency rating (PER) of each player (*514* in total). PER is an advanced metric used in basketball to measure the overall rating of a player’s per-minute statistical production. The formula for PER is quite complex but, in simple terms, it sums up all the good things a player does and subtracts negative things a player does.
3.  The **Player Salaries** data set presents the salaries of all NBA players (*516* in total) for the 2019-2020 season.


After data cleaning and feature engineering, the final compiled data set looked like:

![Tiers](https://github.com/xavier-lim/hiddenbasket/blob/master/images/Tiers.PNG)

---

As you can see from the boxplots, LD1 effectively distinguished the tiers. The higher the LD1 score, the higher the salary tier.

![LD](https://github.com/xavier-lim/hiddenbasket/blob/master/images/LD.png)

## Tableau Project Dashboards
Interactive Version: [HiddenBasket Dashboards](https://xavier-lim.github.io/HiddenBasketDashboards.html)

![Correlations](https://github.com/xavier-lim/hiddenbasket/blob/master/images/correlations.png)

---

![Bigs](https://github.com/xavier-lim/hiddenbasket/blob/master/images/bigs.png)

---

![Guards](https://github.com/xavier-lim/hiddenbasket/blob/master/images/guards.png)

## Conclusion
In conclusion, points per game (PTS), assists per game (AST), rebounds per game (REB), blocks per game (BLK) and player efficiency rating (PER) were used to predict a player's salary tier. Based on the model predictions from the discriminant analysis, I decided to create my undervalued dream team consisting of twelve of the most undervalued NBA players. These players were Tier 1 and Tier 2 players (less than $5 million) with the highest probability of being in Tier 5 (more than $25 million). The following players were selected: John Collins, Domantas Sabonis, Bam Adebayo, Pascal Siakam, Donovan Mitchell, Devonte' Graham, Shai Gilgeoues-Alexander, Jamal Murray, Buddy Hield, Caris LeVert, and Collin Sexton, and Richaun Holmes.

## Acknowledgements
1.	Moneyball, based on a true story about the Oakland Athletics and their general manager Billy Beane who was tasked with assembling a competitive baseball team with a limited salary budget. He decided to use statistical analysis to find and acquire undervalued baseball players.
2.	John Hollinger, analyst and former Vice President of Basketball Operations for the Memphis Grizzlies developed the player efficiency rating (PER) to produce a per-minute player performance rating. To learn more, visit:  https://www.basketball-reference.com/about/per.html

## Author
* **Xavier Lim** | [LinkedIn](https://www.linkedin.com/in/xavier-lim14/) | [Portfolio Website]( https://xavier-lim.github.io/)

