
# Does Money Buy Wins?
### Payroll Efficiency and Competitive Performance in Major League Baseball (2021–2026)

## Overview

Does spending more money lead to more wins in Major League Baseball?

This independent sports analytics project examines the relationship between team payroll expenditure and regular-season performance across all 30 MLB organizations from 2021 to 2026.

Using 180 team-season observations, I investigate whether financial expenditure predicts competitive success, develop a payroll efficiency index, and simulate how alternative salary cap-and-floor structures could affect financial inequality.

**[Read the Full Research Report](**[Read the Full Research Report](Does%20Money%20Buy%20Wins%20Payroll%20Efficiency%20and%20CompetitivePerformance%20in%20Major%20League%20Baseball%20%282021%E2%80%932026%29.pdf)**)**

## Tools & Methods

**Language:** R  
**Libraries:** tidyverse, dplyr, ggplot2, knitr, kableExtra  
**Reporting:** R Markdown, LaTeX, PDF

Statistical methods include:
- Pearson correlation and simple linear regression
- Year-over-year payroll and performance comparisons
- Development of a custom payroll efficiency index
- Sensitivity analysis and Spearman rank correlation
- Salary cap-and-floor simulations
- Gini coefficient analysis
- Comparative organizational case studies

## Key Findings

### 1. Payroll Has Limited Predictive Power

Across 180 team-season observations, payroll exhibited a positive correlation with regular-season victories:

- **Pearson's r:** 0.3417
- **R²:** 0.1168

Payroll explained approximately 11.7% of the variation in regular-season wins under a simple linear regression model.

### 2. Increased Spending Does Not Guarantee Improvement

Year-over-year payroll changes showed virtually no linear relationship with changes in victories:

- **Pearson's r:** -0.0778
- **R²:** 0.0061

Changes in payroll explained approximately 0.61% of the variation in changes in wins.

### 3. Payroll Efficiency Varies Across Organizations

I developed a payroll efficiency index measuring victories above the leaguewide average per $1 million in payroll.

The highest-ranked organizations across 2021–2026 were:

| Rank | Organization | Average Efficiency |
|------|--------------|-------------------:|
| 1 | Tampa Bay Rays | 0.1220 |
| 2 | Milwaukee Brewers | 0.1180 |
| 3 | Los Angeles Dodgers | 0.0756 |

Sensitivity analyses demonstrated that rankings were more sensitive to the selected win benchmark than to the method used to aggregate annual efficiency.

### 4. Payroll Inequality Can Be Reduced Without Guaranteeing Competitive Balance

Three hypothetical salary cap-and-floor scenarios were applied to 2026 payroll data.

The original payroll Gini coefficient of **0.2360** declined to:

- **0.0846** under Scenario A
- **0.0676** under Scenario B
- **0.1823** under Scenario C

These simulations measure changes in payroll distribution, not predicted changes in team victories.

### 5. Similar Spending Does Not Guarantee Similar Outcomes

Comparative case studies examined the Milwaukee Brewers, Tampa Bay Rays, Los Angeles Dodgers, and New York Mets.

The Dodgers and Mets maintained similarly substantial payrolls but achieved markedly different competitive outcomes. Meanwhile, the Brewers and Rays demonstrated strong payroll-adjusted performance with considerably smaller financial commitments.

## Limitations

The analysis is descriptive and does not establish causation. Results depend on payroll definitions, the selected efficiency benchmark, and the 2021–2026 observation period.

Salary cap-and-floor simulations assume immediate compliance and do not model roster changes, contract obligations, or future competitive outcomes.

## Repository Contents

- `Does_Money_Buy_Wins.pdf` — Complete research report
- `MLB_Payroll_Analysis.Rmd` — R Markdown source code
- `data/MLB_Salaries.xlsx` — Dataset used in the analysis, if redistribution is permitted

## Data Sources

- The Baseball Cube — MLB payroll data
- MLB regular-season standings data
- Major League Baseball — November 2026 salary cap-and-floor proposal

## Conclusion

Financial expenditure is positively associated with regular-season success, but payroll alone explains a relatively small proportion of performance variation.

**Money may provide opportunities to win, but spending alone does not guarantee success.**

---

**Author:** Borna Anic-Matic  
**Project Type:** Independent Sports Analytics Research  
**Period Analyzed:** 2021–2026
