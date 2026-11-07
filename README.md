
# Does Money Buy Wins? An Analysis of Payroll Efficiency in Major League Baseball (2021–2026)

## Project Overview

Following the Milwaukee Brewers' 2026 World Series championship and ongoing discussions surrounding the potential introduction of salary caps and payroll floors in Major League Baseball, this project investigates an important question:

**To what extent does a team's payroll predict its regular-season success?**

Using data from 30 MLB teams across six seasons (2021–2026), this independent statistical analysis examines the relationship between financial spending and team performance.

Beyond investigating whether higher payrolls are associated with more wins, the project explores whether year-over-year increases in spending correspond with improvements in performance and develops a custom payroll efficiency index to identify organizations that consistently achieve strong results relative to their financial resources.

## Research Questions

1. To what extent does team payroll predict regular-season wins and losses?
2. Are year-over-year changes in payroll associated with changes in team performance?
3. Which MLB organizations achieve the greatest regular-season success relative to their payroll?
4. How sensitive are payroll efficiency rankings to the assumptions used to construct the index?
5. What insights can payroll efficiency provide when evaluating hypothetical MLB salary caps and floors?

## Dataset

The analysis uses data covering:

- **30 MLB teams**
- **6 seasons (2021–2026)**
- **180 team-season observations**
- **150 potential year-over-year comparisons (2022–2026)**

Key variables include:

- Team payroll (USD)
- Regular-season wins and losses
- Year-over-year payroll changes
- Year-over-year win and loss changes
- Cost per win
- Payroll efficiency scores

Payroll and standings data were compiled into a multi-season dataset and analyzed using R.

## Methodology

### Section 1: Payroll and Regular-Season Performance

The initial analysis examines the relationship between team payroll and regular-season wins and losses using:

- Scatterplots with fitted linear trend lines
- Pearson correlation coefficients
- Coefficients of determination (R²)

### Section 2: Year-Over-Year Changes in Payroll and Performance

The second section investigates whether increases or decreases in spending correspond with changes in regular-season performance.

For each team, changes in payroll, wins, and losses are calculated by subtracting the previous season's values from the current season's values.

Pearson correlations and R² statistics are used to evaluate the strength of these relationships.

### Section 3: Developing a Payroll Efficiency Index

The third section introduces a custom metric to evaluate how effectively MLB organizations convert financial resources into regular-season success.

The initial measure, **cost per win**, is calculated as:

Cost per Win = Team Payroll / Regular-Season Wins

However, this calculation can favour teams with low payrolls even when they finish with losing records.

To address this limitation, a revised payroll efficiency index was developed:

**Efficiency Score = (Team Wins − League Average Wins) / Payroll in Millions**

This index measures the number of wins above the league average achieved per $1 million in team payroll.

- Positive scores indicate above-average performance.
- Negative scores indicate below-average performance.
- Higher scores indicate greater payroll-adjusted success under the index.

Annual scores are calculated for each team, followed by six-year averages to evaluate organizational consistency.

## Preliminary Findings

### 1. Payroll and Regular-Season Performance

Team payroll demonstrated a positive relationship with wins and a negative relationship with losses.

| Relationship | Pearson's r | R² |
|---|---:|---:|
| Payroll vs. Wins | 0.3417 | 0.1168 |
| Payroll vs. Losses | -0.3431 | 0.1177 |

Payroll explained approximately **11.68% of the variation in regular-season wins** and **11.77% of the variation in losses** in the pooled simple linear models.

These findings suggest that payroll alone has relatively limited explanatory power when evaluating regular-season performance.

### 2. Payroll Changes and Performance Changes

Year-over-year payroll changes demonstrated very weak linear relationships with changes in wins and losses.

| Relationship | Pearson's r | R² |
|---|---:|---:|
| Payroll Change vs. Wins Change | -0.0759 | 0.0058 |
| Payroll Change vs. Losses Change | 0.0781 | 0.0061 |

Changes in payroll explained approximately **0.58% of the variation in year-over-year win changes** and **0.61% of the variation in loss changes**.

These results suggest that increasing team spending is not strongly associated with immediate improvements in regular-season performance across the dataset.

### 3. Payroll Efficiency Rankings (2021–2026)

The custom efficiency index identified the following organizations as the most efficient across the six-season period.

| Rank | Team | Average Efficiency Score |
|---:|---|---:|
| 1 | Tampa Bay Rays | 0.1220 |
| 2 | Milwaukee Brewers | 0.1180 |
| 3 | Los Angeles Dodgers | 0.0756 |
| 4 | Cleveland Guardians | 0.0702 |
| 5 | Atlanta Braves | 0.0585 |
| 6 | Houston Astros | 0.0551 |
| 7 | Seattle Mariners | 0.0539 |
| 8 | New York Yankees | 0.0428 |
| 9 | Philadelphia Phillies | 0.0341 |
| 10 | Toronto Blue Jays | 0.0323 |

#### Key Observations

**Milwaukee Brewers**

- Ranked among the five most efficient teams in five of six seasons.
- Ranked first in 2024, 2025, and 2026.
- Finished second overall in six-year average efficiency.

**Tampa Bay Rays**

- Ranked first in average efficiency across the six-season period.
- Recorded particularly high efficiency scores in 2021 and 2023.
- Demonstrated that strong regular-season performance can be achieved with relatively modest payrolls.

**Los Angeles Dodgers**

- Finished third overall despite operating with substantially larger payrolls.
- Demonstrated that high spending does not necessarily prevent an organization from achieving strong payroll-adjusted performance.

**New York Mets**

- Did not appear among the annual top-five efficiency rankings despite being a high-spending organization.
- Provide an interesting comparison with the Dodgers when evaluating financial resources and competitive outcomes.

These findings suggest that financial efficiency varies considerably among MLB organizations, although the results depend on the specific definition of efficiency used.

## Project Progress

**Status: In Progress**

### Completed

- [x] Data collection and preparation
- [x] Section 1: Payroll vs. Regular-Season Performance
- [x] Section 2: Year-Over-Year Payroll and Performance Changes
- [x] Section 3: Development and Application of Payroll Efficiency Index
- [x] Annual and Six-Year Efficiency Rankings
- [x] Initial Research Report

### Upcoming

- [ ] Section 4: Sensitivity Analysis and Validation of the Efficiency Index
- [ ] Section 5: Hypothetical MLB Salary Cap and Floor Simulations
- [ ] Section 6: Organizational Case Studies
- [ ] Section 7: Final Discussion and Conclusions

## Tools and Technologies

- **R** — Statistical analysis and calculations
- **RStudio** — Development environment
- **dplyr** — Data manipulation
- **ggplot2** — Data visualization
- **readxl** — Excel data import
- **knitr / kableExtra** — Report tables and formatting
- **R Markdown** — Reproducible research reporting

## Limitations

This analysis is observational and does not establish causal relationships between payroll and team performance.

Factors including player development, injuries, roster construction, coaching, and organizational decisions may influence regular-season outcomes.

Additionally, the custom efficiency index measures wins above league average relative to payroll rather than the true marginal financial cost of generating additional wins. As a result, rankings should not be interpreted as definitive measures of organizational effectiveness.

The pooled dataset also contains repeated observations of the same franchises across seasons, and year-to-year payroll levels may not be directly comparable without further adjustment.

These limitations will be explored through sensitivity analysis in the next stage of the project.

## Future Directions

The next phase of the analysis will evaluate how robust the efficiency rankings are under alternative assumptions and measurement approaches.

The project will subsequently examine hypothetical salary caps and payroll floors, investigating how different financial structures might affect MLB organizations.

Finally, the Milwaukee Brewers, Tampa Bay Rays, Los Angeles Dodgers, and New York Mets will be examined as organizational case studies to compare different approaches to team spending and competitive success.

## Author

Borna Anic-Matic

Independent Baseball Analytics Project | R | 2026
