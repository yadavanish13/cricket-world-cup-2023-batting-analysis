# 2023 Cricket World Cup: Batting Analysis

## Goal
Analyze batting performance at the 2023 ICC Men's Cricket World Cup using Python to find the top run scorers, the fastest scorers, the biggest six hitters, and the most consistent batters.

## Dataset
- Source: Kaggle (2023 Cricket World Cup dataset)
- Files used: `BATTING.csv`, `PLAYERS_INFO.csv`
- Rows / columns: [ADD from df.shape]

## Tools
- Python
- pandas (data cleaning, grouping, aggregation)
- matplotlib (bar charts, scatter plot)
- Google Colab

## Key Findings
- **Top run scorer:** Virat Kohli with 765 runs
- **Fastest scorer (min 100 balls faced):** Kusal Mendis with a strike rate of 166.4
- **Most sixes:** Rohit Sharma with 28 [UPDATE after name cleaning]
- **Top team by total runs:** [ADD from team printout]
- **Most consistent batter (min 5 innings):** [ADD top name from average list]

## Charts
1. Top 10 run scorers
2. Best strike rates (min 100 balls)
3. Most sixes
4. Total runs by team
5. Best batting average per innings
6. Runs vs. balls faced (scatter)

(Add the saved PNG images here.)

## Method
1. Loaded the CSV files with `latin1` encoding.
2. Cleaned column names and player names, and converted numeric columns with `pd.to_numeric`.
3. Grouped by player to compute totals and strike rate (runs / balls x 100).
4. Applied minimum thresholds (100 balls, 5 innings) so small samples do not skew rankings.
5. Merged with player info to get team-level totals.

## What I Learned
- Cleaning data first (spaces, data types, name tags) matters more than the charts.
- Minimum-sample filters are needed for fair strike rate and average comparisons.
- Merging tables can silently lose rows, so always check for missing matches.

## Next Steps
- Bowling analysis using `BOWLING.csv`
- Match-level analysis using `Cricket_WC23.csv`
- Interactive dashboard (Streamlit or Power BI)
