# Attacking Creator Recruitment Analysis | 2024/25

**Python | SQL | DuckDB | pandas | Matplotlib**

## Project Overview

This project evaluates attacking creators from Europe's five major football leagues using 2024/25 player-performance data.

The objective was to develop a reproducible statistical screening process that could help a recruitment department identify players for further scouting.

Rather than ranking players solely by goals or assists, the analysis combines chance creation, scoring threat, and involvement in attacking buildup.

## Analytical Approach

The analysis uses Understat player-season statistics obtained from the publicly available [Understat Players Aggregated dataset](https://github.com/vibedatascience/understat_players_aggregated).

SQL was used to filter and aggregate the data, while Python and pandas were used to calculate performance metrics, construct weighted rankings, and evaluate the results.

The model considers four per-90-minute statistics: expected assists (xA), key passes, non-penalty expected goals (npxG), and expected goals buildup (xG buildup).

Three recruitment strategies were tested: Balanced, Creation-first, and Goal-threat emphasis.

An initial minimum of 1,200 minutes was increased to 1,800 minutes to assess the stability of the player rankings.

## Key Findings

The initial screening identified 282 player-league records. Applying the stricter playing-time threshold reduced this to 174.

Seven players appeared in the top 10 across all three recruitment strategies.

Michael Olise ranked first in every model, recording 0.543 xA and 0.381 npxG per 90 minutes during the 2024/25 season.

Julian Brandt and Martin Ødegaard showed consistent results in the creativity-focused comparisons.

Maghnes Akliouche also appeared in all three top tens, making him a candidate for further tactical and video analysis.

## Recruitment Recommendation

Use the seven consistently high-ranked players as a statistical reference group for further scouting.

The rankings identify attacking production, but they do not establish which player would be the best signing. Positional responsibilities, tactical suitability, defensive contributions, financial constraints, and transfer feasibility should be evaluated before making recruitment decisions.

## Tools and Methods

Python, pandas, DuckDB SQL, Matplotlib, data quality validation, per-90 normalization, percentile-based scoring, sensitivity analysis, and comparative visualization.

## Notebook

[View the complete recruitment analysis](01_soccer_recruitment_analysis.ipynb)

The notebook includes the data preparation process, SQL queries, exploratory visualizations, player rankings, sensitivity tests, and final scouting report.

To reproduce the results, open the notebook in Google Colab and run all cells. The notebook references a fixed dataset revision for reproducibility.

## Limitations

The model uses analyst-defined weights, broad positional classifications, and performance data from different leagues without fully adjusting for league strength or tactical context.

Results should therefore be interpreted as a preliminary scouting screen, not a prediction of transfer success.

## Author

**Juan Vasquez**

M.S. Information Systems — Data Analytics

B.S. Recreation & Sports Management

Interested in sports performance analytics, business intelligence, and data-driven decision-making.
