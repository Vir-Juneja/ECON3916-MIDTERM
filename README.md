# ECON3916-MIDTERM-PROJECT
# NFL Home Attendance and Winning, 2010–2019

ECON 3916 Midterm Project · Vir Juneja


## Question

For NFL teams from 2010 to 2019, how does a team's winning percentage in a season relate to its average home attendance per game, holding last season's winning percentage, the size of its metro area, the team and the year fixed?

## Data

| File / source | What it holds |
|---|---|
| `data/attendance.xlsx` | Pro Football Reference weekly attendance tables, 2010–2019, one sheet per season, exported by hand. Example page: https://www.pro-football-reference.com/years/2019/attendance.htm |
| nflverse games file (downloaded by the notebook) | Every regular-season score, used to calculate win %, 2009–2019: https://github.com/nflverse/nfldata. Checked against Pro Football Reference's 2019 standings. |
| Census Bureau metro population estimates (downloaded by the notebook) | Population of each metro area, 2010–2019: https://www2.census.gov/programs-surveys/popest/datasets/2010-2019/metro/totals/cbsa-est2019-alldata.csv |

The final dataset has 320 rows (32 teams × 10 seasons), one row per team-season, with no missing values.

## How to run

1. Open `Midterm Project/Econ_3916_Midterm.ipynb` in Google Colab (use the link above, or File › Open notebook › GitHub and search for this repo).
2. Click **Runtime › Run all**.
3. The notebook reads `data/attendance.xlsx` straight from this repository and downloads the nflverse and Census files itself, so nothing needs to be uploaded. It needs an internet connection and takes about a minute.

Every number in the report is printed by the notebook's last code cell, "Numbers my report quotes."

## Headline finding

Within a team, a 0.1 rise in this season's win % (about 1.6 more wins) goes with about 137 more fans per home game, but the 95% interval for the full coefficient (−968 to 3,706, clustered by franchise) includes zero. Last season's record matters more: a 0.1 rise goes with about 458 more fans per game (95% interval 1,666 to 7,484). N = 320 team-seasons. Both are conditional associations, not causal effects.

## Repository contents

- `README.md`: this file
- `data/attendance.xlsx`: the attendance data
- `Midterm Project/Econ_3916_Midterm.ipynb`: the analysis notebook
- `Midterm Project/midterm-report.pdf`: the written report

# Question
For NFL teams from 2010-2019, how is teams winning percentage associated with how many fans come to its home games, controlled for last seasons winning percentage and the size of its metro area.

## Data
- **Attendance:** Pro Football Reference weekly attendance pages, 2010–2019,
  saved as `data/attendance.xlsx` (one sheet per season).
  Example page: https://www.pro-football-reference.com/years/2019/attendance.htm
- **Win %:** calculated from game results in the nflverse games file,
  https://github.com/nflverse/nfldata
- **Metro population:** Census Bureau metro area population estimates, 2010–2019,
  https://www2.census.gov/programs-surveys/popest/datasets/2010-2019/metro/totals/cbsa-est2019-alldata.csv

  ## How to run
  1. Open Midterm Project/Econ_3916_midterm.ipynb in Colab
  2. Click Runtime > Run All
  3. The notebook reads all data straight from the repo, it takes about a minute.
 
  All numbers in this report are printed by the notebooks last code cell, Numbers my report quotes.

  ## Headline finding
Within a team, a 0.1 rise in this season's win % (about 1.6 more wins) goes with about 137 more fans per home game, but the 95% interval for the full coefficient (−968 to 3,706, clustered by franchise) includes zero. Last season's record matters more: a 0.1 rise goes with about 458 more fans per game (95% interval 1,666 to 7,484). N = 320 team-seasons. Both are conditional associations, not causal effects.

## Repository contents

- `README.md`: this file
- `data/attendance.xlsx`: the attendance data
- `Midterm Project/VirMidterm.ipynb`: the analysis notebook
- `Midterm Project/Vir3916Midterm.pdf`: the written report

