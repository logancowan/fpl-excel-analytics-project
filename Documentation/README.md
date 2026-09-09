# FPL Analytics Model — Methodology

## Project Objective

The objective of this project is to develop a data-driven Fantasy Premier League analytics model that evaluates player performance, fixture difficulty, player value and squad selection.

The model combines statistical player metrics with fixture analysis to estimate expected player performance and support squad optimisation.

## Data

The model uses up to date Fantasy Premier League player and fixture data.

Key player-level variables include:

- Player position
- Team
- Price
- Minutes
- Starts
- Total Points
- Points per 90
- Expected Goals (xG)
- Expected Assists (xA)
- Expected Goal Involvement (xGI)
- Bonus
- Defensive Contributions
- Clean Sheets

Historical premier league season data is also included within the Excel model, but have disgarded data players have at clubs outside of the premier league, to attempt to avoid misleading results from aspects such as coventry players winning the league last year, so would have inflated data.

## Player Modelling

Player performance is evaluated using a combination of historical performance and underlying attacking and defensive metrics.

The model i made considers:

- Points per 90
- xG per 90
- xA per 90
- xGI per 90
- Points per £m
- xGI per £m
- Starting probability
- Defensive contribution potential
- Bonus potential
- Reliability
- Fixture difficulty

These variables are combined to produce a model-based expected points estimate for upcoming weeks.

## Fixture Modelling

Fixtures are incorporated into the player model through team and opponent strength measures.

Fixture adjustments consider:

- Team attacking strength
- Team defensive strength
- Opponent attacking strength
- Opponent defensive weakness
- Expected goals
- Fixture difficulty

The resulting fixture adjustment is incorporated into player expected performance.

## Squad Optimisation

The model uses the player scores to construct an optimised 15-player squad.

The optimisation considers standard FPL squad constraints, including:

- 2 goalkeepers
- 5 defenders
- 5 midfielders
- 3 forwards
- £100m budget
- Maximum 3 players from one club

## Power BI Dashboard

Power BI is used to transform the model outputs into an interactive decision-support dashboard, and to highlight results found in the excel model.

The dashboard contains:

### FPL Overview

A high-level view of player performance, including player rankings, top scorers, top assisters and the relationship between player price and model expected points, giving an insight into wether perhaps it is more valuable to spend more of a budget on an attacking player or a defensive player.

### Player Analysis

Allows individual players to be investigated using performance metrics, model expected points, value metrics and fixture outlook, and shows a players expected points breakdown, i.e. is a player likely to get there points from goals or defensive contributions etc.

### Squad Optimisation

Displays the optimised squad , squad cost, expected points, remaining budget, and squad composition according to the model and the data up to the point. Obviously data can only be useful in the aid of prediciting most likely outcomes, and who is most likely to perform the best, but the model can be used to help aid a FPL players decision making to attempt to maximise performance.

## Model Validation

Historical model validation is planned as a future development stage, to predict points gameweek by gameweek as oppose to an average of the next 6 which all though may be more accurate maybe more useful to do week by week to maximise team selection of say rotational players if one week a player has a good fixture then next does not, finding if there is a good rotational option or not. 

Plan to in future note up to 20 of the model highest position rank players for each positions predicted points for a few gameweeks and compare them to what they do actually achieve, to be able to analyse the data and then work on the model to see if there are any other potential improvements to the model, for example maybe considering factors of home and away fixtures. 
Planned potential metrics to analyse include:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Correlation
- Rank correlation
- Top-10 hit rate

## Future Development

Future development will focus on historical backtesting, model calibration and further evaluation of player ranking performance across previous FPL seasons. The data for the model as of current is low for the season and view it as a project to perfect for the end of gameweek 18 to then be able to fully use as team selection for a wilcard (where you get unlimited free transfers) and maximise my team performance.
