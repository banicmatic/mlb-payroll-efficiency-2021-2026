
# Does Money Buy Wins?
### Payroll Efficiency, Competitive Performance, and Financial Inequality in Major League Baseball (2021–2026)

**Independent Sports Analytics Project | R | 2026**

## Overview

Does spending more money lead to more wins in Major League Baseball?

This independent research project examines the relationship between MLB team payroll and regular-season performance from 2021 to 2026. Using data from all 30 MLB organizations, the analysis investigates whether higher spending translates into greater competitive success, identifies organizations achieving strong results relative to their financial resources, and explores the economic implications of salary caps and payroll floors.

The project extends beyond correlation analysis by developing a payroll efficiency index, testing its robustness, and simulating alternative leaguewide spending structures.

## Methods & Tools

**Language:** R  
**Libraries:** `dplyr`, `tidyr`, `ggplot2`, `readxl`, `knitr`, `kableExtra`, `ineq`

**Statistical techniques:**
- Pearson correlation and simple linear regression
- Year-over-year payroll and performance analysis
- Development of a payroll efficiency index
- Sensitivity analysis and Spearman's rank correlation
- Salary cap and payroll floor scenario modelling
- Gini coefficient analysis of payroll inequality

## Key Findings

- **Payroll and Wins:** Team payroll explained approximately **11.68%** of the variation in regular-season wins in a simple linear model.
- **Changes in Spending:** Year-over-year payroll changes exhibited very weak linear relationships with changes in team performance.
- **Payroll Efficiency:** The Tampa Bay Rays and Milwaukee Brewers ranked first and second in average payroll efficiency across the six-season period.
- **Methodological Robustness:** Alternative aggregation methods produced highly similar organizational rankings, with Spearman's rank correlation of **0.9938**.
- **Salary Regulations:** Applying MLB's reported November 2026 salary cap-and-floor thresholds produced an illustrative **$263.72 million net increase** in leaguewide payroll and reduced the simulated Gini coefficient from **0.2360 to 0.0846**.

## Limitations

The analysis identifies statistical associations rather than causal relationships. The payroll efficiency index is sensitive to the selected performance baseline, and the financial simulations assume immediate compliance with the spending restrictions. The dataset's payroll accounting may also differ from MLB's Competitive Balance Tax methodology.

## Repository Contents

- `PayrollAnalysisBaseball.Rmd` — R Markdown source code and analysis
- `PayrollAnalysisBaseball.pdf` — Full research report
- `MLB Salaries.xlsx` — Dataset used for the analysis

## Project Status

**Work in Progress — Sections 1–5 Completed**

Upcoming work includes comparative organizational case studies of the Milwaukee Brewers, Tampa Bay Rays, Los Angeles Dodgers, and New York Mets, followed by the final discussion and conclusions.

---

*An independent research project exploring the intersection of baseball analytics, statistical methodology, and sports economics.*
