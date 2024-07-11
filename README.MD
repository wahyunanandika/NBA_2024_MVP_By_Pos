# Analyzing Player Position Value in Modern NBA Trends
## Introduction

The Objectives of this analysis is to identify the most impactful player positions in NBA and relate them to the evolving trends of modern basketball, in the context of this analysis, modern basketball refers to NBA gameplay characterized by evolving player roles, and fast pace game. Modern basketball emphasize versatility, speed, and skills in all positions, while on the other hand older basketball, which often featured more structured play, centred around post-up offense, and distinct positional roles. The dataset used contain statistics of NBA players across different positions, focusing on points per game, assists per game, rebounds per game, foul committed, steals per game, blocks per game, age and height categories. 

## Datasets

The dataset used is from (https://www.basketball-reference.com/leagues/NBA_2024_per_game.html), representing the NBA 2023-2024 season. This dataset contains 572 entries, each representing a player based on the team he played for that season. It includes 29 columns representing player name, age, position, games played, games started (played as part of the starting five), minutes per game, field goals per game, field goal attempts per game, field goal percentage, three-point field goals per game, three-point field goal attempts per game, three-point field goal percentage, two-point field goals per game, two-point field goal attempts per game, two-point field goal percentage, effective field goal percentage (this statistic adjusts for the fact that a three-point field goal is worth one more point than a two-point field goal), free throws per game, free throw attempts per game, free throw percentage, offensive rebounds per game, defensive rebounds per game, total rebounds per game (offensive rebounds + defensive rebounds), assists per game, steals per game, blocks per game, turnovers per game, personal fouls per game, and points per game. From this dataset, the variables of interest are points scored, assists, rebounds, fouls committed, steals, and blocks.

## Research Question 1

First research question explores the averages performances metric of NBA players in term of points scored, assists, rebounds, fouls committed, steals, blocks, with the aim to identifying which player positions contribute most significantly to these statistics. This analysis will help basketball fans and enthusiasts understand the impact of different positions on overall team performances.

### Average Performance Metrics By Position

1. Points Per Game (PTS) :
    - Point Guard (PG) : 10.36
    - Shooting Guard (SG) : 8.15
    - Small Forward (SF) : 7.89
    - Power Forward (PF) : 9.34
    - Center (C) : 8.81

2. Total Rebounds Per Game (TRB) :
    - Point Guard (PG) : 2.82
    - Shooting Guard (SG) : 2.38
    - Small Forward (SF) : 3.24
    - Power Forward (PF) : 4.25
    - Center (C) : 5.99

3. Assists Per Game (AST) :
    - Point Guard (PG) : 3.85
    - Shooting Guard (SG) : 1.99
    - Small Forward (SF) : 1.48
    - Power Forward (PF) : 1.81
    - Center (C) : 1.57

4. Steals Per Game (STL) :
    - Point Guard (PG) : 0.83
    - Shooting Guard (SG) : 0.59
    - Small Forward (SF) : 0.64
    - Power Forward (PF) : 0.63
    - Center (C) : 0.54

5. Fouls Per Game:
    - Point Guard (PG) : 2.93
    - Shooting Guard (SG) : 2.27
    - Small Forward (SF) : 2.38
    - Power Forward (PF) : 2.69
    - Center (C) : 3.14

6. Blocks Per game (BLK) :
    - Point Guard (PG) : 0.25
    - Shooting Guard (SG) : 0.26
    - Small Forward (SF) : 0.34
    - Power Forward (PF) : 0.52
    - Center (C) : 0.89

### Variances In Points Per Game Per Position:

- Point Guard (PG) : 68.44
- Shooting Guard (SG) : 45.59
- Small Forward (SF) : 35.91
- Power Forward (PF) : 53.81
- Center (C) : 44.23

Interpretation : The variance indicates the spread of points scored by players in each position. Point guards have the highest variance, meaning there is a larger range in their scoring performances compared to other positions. This could be due to the diverse roles point guards play, from being primary scorers to facilitators.

### Max Points per Game By Positions:

- Point Guard (PG) : 33.9
- Shooting Guard (SG) : 26.60 
- Small Forward (SF) : 24.0
- Power Forward (PF) : 30.40
- Center (C) : 34.70

Interpretation : The maximum points per game highlight the peak scoring performances within each position. Centers and point guards have the highest maximum points, indicating that individual players in these positions have the potential for high-scoring games.

### Distribution Players by positions in NBA:

- Point Guard (PG) : 18.1%
- Shooting Guard (SG) : 23.8%
- Small Forward (SF) : 21.5%
- Power Forward (PF) : 19.4%
- Center (C) : 17.1%

### Summary

The analysis of average performance metrics reveals that Point Guard (PG) have the highest average point per game (10.36) and assists per game (3.85), indicating their crucial role in scoring and playmaking. Centers (C) lead in total rebounds (5.99) and blocks (0.89), highlighting their defensive and rebounding capabilities. Shooting Guards (SG) and Small Forward (SF) contribute significantly across various metrics, with notable performances in points and steals. Power Forward (PF) demonstrate balanced contribution in rebounds and blocks.

When it come foul committed, Point Guards (PG) have high average 2.93 fouls per game, reflecting their role in coordinating aggressive offensive plays. Centers  (C), with the highest average of 3.14 fouls per game, often engage in physical defense and tactical fouling strategies to disrupt the opponents.

The Larger distribution of Shooting Guards (SG) and Small Forwards (SF) in the NBA (23.8 % and 21.5 % respectively) reflects the modern NBA’s emphasis on wing players who can excel in both scoring and defense. These positions are crucial in “3-and-D” role, combining three point shooting prowess with defensive skills to enhance team performances.

By examining the distribution of players	by position, we can see that Shooting Guard (SG) are the most common, followed by Small Forward (SF) and Point Guards (PG). This distribution reflects evolving trend in modern basketball, where versatility and skill are emphasized across all positions.

## Research Question 2

This Research question examines the relationship between player age, height category, and points scored per game (PTS) in hte NBA. Understanding correlation between these provide insight into how age and height influence scoring performances.

To categorize height, I split players into three categories based on their positions: guards (PG, SG) for shorter players, forwards (SF, PF) for medium-height players, and centers (C) for taller players.

### Covariance Matrix

|           |Height Category|Age|PTS|
|-----------|---------------|---|---|
|Height Category|0.529030|0.202499|-0.130436|
|Age|0.202499|17.311145|4.051237|
|PTS|-0.130436|4.051237|49.238054|

The covariance matrix shows the covariances values between height category, age, and point scored (PTS):

    - Height Category : There is a positive covariance of 0.529 between height category number and age, indicating a slight tendency    for older players to be in higher height categories
    - Age : The covariance between age and points scored (PTS) is 4.051, suggesting a moderate positive relationship where older players tend to score more points.
    - Points : The covariance between points scored (PTS) and height category number is -0.130, indicating a weak negative relationship where taller players in higher height categories may score slightly fewer points.

### Correlation Matrix

|           |Height Category|Age|PTS|
|-----------|---------------|---|---|
|Height Category|1.000000|0.067006|-0.025514|
|Age|0.067006|0.067006|0.067006|
|PTS|0.067006|0.067006|0.067006|

The correlation matrix provides correlation coefficients, which standardize the relationships between variables:

    - Height Catergory : The correlation coefficient with age is 0.067, suggesting a very weak positive relationship between height category number and age.
    - Age : The correlation coefficient with points scored (PTS) is 0.139, indicating a weak positive relationship where older players tend to score slightly more points.
    - Points : The correlation coefficient with height category number is -0.026, suggesting a negligible negative relationship between height category number and points scored (PTS).

### Summary

The analysis reveals several insights into the relationships between age, height category, and points scored in the NBA:

    - Older players tend to score slightly more points per game, as indicated by the positive covariance and correlation with age.
    - There is a weak negative relationship between height category number and points scored, suggesting that taller players in higher height categories may score slightly fewer points, though this relationship is not strong.
    - The covariance and correlation values provide a nuanced view of how age and height category influence scoring performance, highlighting the complex dynamics of player statistics in professional basketball.

## Research Question 3

### Hypothesis Testing (Differences in Player Performances based on Age)

Age :

+ Younger player <= 25
+ Older PLayer > 25

1. Rebounds :

    - Null Hypothesis (H0): There is no significant difference in rebounds between younger and older players.
    - Alternate Hypothesis (H1): There is a significant difference in rebounds between younger and older players.

2. Asissts (AST) :

    - Null Hypothesis (H0): There is no significant difference in assists between younger and older players.
    - Alternate Hypothesis (H1) : There is a significant difference in assists between younger and older players.

3. Stocks (Steals + Blocks)

    - Null Hypothesis (H0): There is no significant difference in stocks (steals + blocks) between younger and older players.
    - Alternate Hypothesis (H1) : There is a significant difference in stocks (steals + blocks) between younger and older players.

### Summary

1. Rebounds :

    - T-Statistics : -3.6723
    - P-Value : 0.0003
    - Conclusion : Reject the null hypothesis (H0). There is a significant difference in rebounds between younger and older players.

2. Assists : 

    - T-Statistics : -3.8014
    - P-Value : 0.0002
    - Conclusion : Reject the null hypothesis (H0). There is a significant difference in assists between younger and older players.

3. Stocks (Steals + Blocks) :

    - T-Statistics : -3.5198
    - P-Value : 0.0005
    - Conclusion : Reject the null hypothesis (H0). There is a significant difference in stocks between younger and older players.

These results indicate that there are statistically significant differences in rebounds, assists, and stocks (steals + blocks) between younger and older NBA players. Specifically, younger players tend to have different performance levels compared to older players in these metrics.

## Conclusion

The analysis of NBA player statistics highlights significant differences in performance metrics across player positions, with Point Guards leading in scoring and assists, Centers in rebounds and blocks, and Shooting Guards and Small Forwards contributing significantly across various metrics. Age influences scoring dynamics, with older players generally scoring more points per game. Hypothesis testing confirms age-related differences in rebounds, assists, and combined steals and blocks (stocks), underscoring varied player roles and development stages in professional basketball. These insights deepen our understanding of player contributions and strategic roles in modern NBA gameplay.

## Further Research

Further research could explore the integration of machine learning or deep learning models to predict MVP candidates based on voting patterns, player origins, demographic factors such as college attended, and fan engagement metrics. This approach could provide deeper insights into player performance and fan preferences in the evolving landscape of modern basketball. Additionally, incorporating player hot and cold zones or efficiency ratings would enhance the analysis by revealing where players are most effective on the court and how efficiently they contribute to their team's success.

## References

- https://www.stat.cmu.edu/capstoneresearch/315files_s24/team5.pdf
- https://www.stat.cmu.edu/capstoneresearch/
- https://nba-mvp-predictor.streamlit.app/
- [Predicting the 2022–2023 NBA MVP Using Python](https://www.samford.edu/sports-analytics/fans/2023/Using-Machine-Learning-to-Predict-the-NBA-MVP#:~:text=To%20solve%20this%20problem%2C%20a,will%20be%20Nikola%20Jokic%20again)
- https://towardsdatascience.com/predicting-the-nba-mvp-with-machine-learning-c3e5b755f42e
- https://medium.com/@atharvjoshi/predicting-the-2022-2023-nba-mvp-using-python-76cabf4422fd