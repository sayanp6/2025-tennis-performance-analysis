# 2025 Tennis Performance Analysis

## Project Overview

This project analyses the relationship between pre-tournament ATP rankings and men's singles performance across the four 2025 Grand Slam tournaments.

The analysis examines whether players' positions in the ATP rankings were associated with the stage of the tournament they ultimately reached, while also identifying players who performed above or below their ranking-based expectations.

## Research Question

**How closely did pre-tournament ATP rankings relate to men's singles performance across the 2025 Grand Slam tournaments?**

## Tournaments Analysed

- Australian Open
- Roland Garros
- Wimbledon
- US Open

Each tournament contains 128 men's singles players, giving a total of 512 player-tournament observations.

## Methodology

Players were assigned an analyst-defined expected tournament round based on their ATP ranking immediately before each Grand Slam.

| ATP Ranking | Expected Round | Expected Score |
|---|---|---:|
| 1–2 | Final | 7 |
| 3–4 | Semi-final | 6 |
| 5–8 | Quarter-final | 5 |
| 9–16 | R16 | 4 |
| 17–32 | R32 | 3 |
| 33–64 | R64 | 2 |
| 65+ | R128 | 1 |

The expected score provides a numerical measure of the stage a player was expected to reach.

Actual tournament performance was converted into the same scoring system, with the tournament winner receiving a score of 8.

### Performance Deviation

Performance Deviation was calculated as:

**Performance Deviation = Actual Score − Expected Score**

- Positive value = performed above expectation
- Zero = matched expectation
- Negative value = performed below expectation

The expected-performance methodology is an analyst-defined framework and does not represent an official ATP prediction.

## Analysis

The project combines several analytical approaches:

### Excel and Power Query

- Data importing and cleaning
- Power Query transformations
- Tournament and player-level data preparation
- Expected vs actual performance analysis
- Tournament comparisons
- Descriptive statistics
- Correlation analysis
- Regression analysis
- Dashboard visualisation

### Python

Python and pandas were used for additional analysis, including:

- ATP ranking-group comparisons
- Average actual performance by ranking group
- Performance deviation by ranking group
- Cross-tournament player analysis
- Aggregation and statistical analysis

### SQL

SQL was used to practise querying and analysing the tennis dataset, including filtering, grouping and aggregating player and tournament-level information.

## Statistical Analysis

The project examines:

- Average expected and actual performance
- Performance deviation
- Variation in performance
- Correlation between ATP ranking and actual performance
- Correlation between expected and actual scores
- Linear regression between Expected Score and Actual Score

The regression model takes the form:

**Actual Score = Intercept + Coefficient × Expected Score**

## Data Sources

The underlying tennis data comes from the Jeff Sackmann ATP tennis dataset and an archival mirror of that data.

The dataset provides ATP rankings, tournament results, player information and match-level results.

Source repositories:

- Jeff Sackmann ATP Tennis Data
- Aneeshers Tennis Sackmann Archive
- ATP player reference data

## Limitations

The analysis has several limitations:

- ATP rankings provide a measure of player standing but cannot account for every factor affecting tournament performance.
- The expected-round methodology is analyst-defined rather than an official ATP forecasting model.
- Injuries, withdrawals, surface preferences, draw difficulty and individual match-ups are not explicitly modelled.
- Some players may not have had an active ATP ranking immediately before a tournament due to protected-ranking or other circumstances.
- Correlation and regression results identify statistical relationships but do not establish causation.

## Tools Used

- Microsoft Excel
- Power Query
- Python
- pandas
- SQL
- SQLite
- GitHub

## Project Structure

```text
2025-tennis-performance-analysis/
│
├── README.md
├── Excel/
├── Python/
├── SQL/
└── Data/
