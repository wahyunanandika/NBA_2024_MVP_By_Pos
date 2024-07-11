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
