# Sports Betting Algorithms: Quick Reference Guide

## 1. Data Sources and APIs

### 1.1 Major League APIs
- **MLB**: Pybaseball (Python library for MLB data)
- **NBA**: nba_api (Python library for NBA statistics)
- **NFL**: nflgame (Python library for NFL data)
- **NHL**: nhl_api (Python library for NHL statistics)

### 1.2 Odds and Betting Data
- **OddsAPI**: Historical and real-time betting odds
- **The Odds API**: Historical odds data with line movements
- **Sportradar**: Comprehensive sports data, including odds and player statistics
- **Statsperform**: Advanced analytics and data for multiple sports

### 1.3 Additional Data Sources
- **Sports Reference**: Extensive statistical databases for multiple sports
- **FiveThirtyEight**: Sports predictions and ELO ratings
- **Rotowire**: Player news, injury updates, and projections

## 2. Key Metrics and Advanced Stats

### 2.1 Cross-Sport Metrics
- **ELO Ratings**: Team strength indicator based on game outcomes
- **SRS (Simple Rating System)**: Point differential and strength of schedule metric
- **Pythagorean Expectation**: Expected win percentage based on points scored/allowed

### 2.2 NBA-Specific
- **Net Rating**: Team's point differential per 100 possessions
- **True Shooting Percentage (TS%)**: Shooting efficiency including all shot types
- **Usage Rate**: Percentage of team plays used by a player
- **RAPM (Regularized Adjusted Plus-Minus)**: Player's impact adjusted for teammates and opponents

### 2.3 MLB-Specific
- **wOBA (Weighted On-Base Average)**: Comprehensive offensive metric
- **FIP (Fielding Independent Pitching)**: Pitcher performance independent of fielding
- **WAR (Wins Above Replacement)**: Player's total contribution to their team
- **Statcast Data**: Exit velocity, launch angle, spin rate, etc.

### 2.4 NFL-Specific
- **DVOA (Defense-adjusted Value Over Average)**: Team efficiency compared to league average
- **EPA (Expected Points Added)**: Value of a play based on down, distance, and field position
- **QBR (Quarterback Rating)**: Comprehensive quarterback performance metric
- **CPOE (Completion Percentage Over Expected)**: Quarterback accuracy adjusted for throw difficulty

### 2.5 NHL-Specific
- **Corsi and Fenwick**: Shot attempt differentials
- **PDO**: Sum of shooting percentage and save percentage
- **Expected Goals (xG)**: Goal probability based on shot quality
- **Game Score**: Single-number measure of a player's game performance

## 3. Modeling Techniques and Considerations

### 3.1 Time Series Analysis
- **Hurst Exponent**: Long-term memory of time series data
- **Entropy**: Measure of uncertainty in a system
- **ARIMA Models**: For forecasting time series data
- **Kalman Filters**: For tracking and predicting player/team performance over time

### 3.2 Machine Learning Approaches
- **Gradient Boosting (XGBoost, LightGBM)**: For feature importance and predictions
- **Neural Networks**: For capturing complex non-linear relationships
- **Ensemble Methods**: Combining multiple models for improved accuracy

### 3.4 Feature Engineering
- **Moving Averages**: Recent performance trends
- **Home/Away Splits**: Capturing venue impact
- **Head-to-Head History**: Past performance against specific opponents
- **Rest Days**: Impact of schedule on performance
- **Weather Data**: Especially important for MLB and NFL

## 4. Common Pitfalls and Considerations

### 4.1 Data-Related Issues
- **Sample Size**: Ensure sufficient data for reliable conclusions
- **Data Quality**: Verify data accuracy and consistency
- **Multicollinearity**: Be aware of highly correlated features
- **Outliers**: Properly handle extreme values or performances

### 4.2 Modeling Gotchas
- **Overfitting**: Avoid models that are too complex for the available data
- **Regression to the Mean**: Account for extreme performances likely reverting to average
- **Survivor Bias**: Be cautious of datasets that exclude retired players or relegated teams
- **Autocorrelation**: Account for time-dependent correlations in time series data

### 4.3 Betting Market Dynamics
- **Line Movements**: Understand the causes and implications of odds changes
- **Public Betting Percentages**: Consider the impact of public opinion on lines
- **Sharp Money**: Be aware of significant bets from professional bettors
- **Arbitrage Opportunities**: Look for discrepancies between different sportsbooks

### 4.4 Sport-Specific Considerations
- **Injuries and Lineups**: Especially crucial in NBA and NFL
- **Pitching Rotations**: vital for MLB betting
- **Back-to-Back Games**: Important factor in NBA and NHL
- **Playoff vs. Regular Season**: Adjusting models for postseason dynamics
