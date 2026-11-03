
# Does Money Buy Wins? An Analysis of Payroll Efficiency in Major League Baseball (2021–2026)

## Project Overview

This project investigates the relationship between team payroll and regular-season performance in Major League Baseball (MLB) from 2021 to 2026. With ongoing discussions surrounding salary caps, payroll floors, and financial competitiveness in MLB, this analysis examines the extent to which team spending predicts success.

Using R, the project explores whether higher-spending teams achieve better regular-season results and whether year-over-year changes in payroll are associated with improvements in team performance.

## Dataset

The analysis covers **30 MLB teams across six seasons (2021–2026)**, representing **180 team-season observations**.

Key variables include:
- Team payroll
- Regular-season wins and losses
- Year-over-year changes in payroll
- Year-over-year changes in wins and losses

## Methodology

The project uses R for data manipulation, visualization, and statistical analysis.

Statistical techniques include:
- Exploratory data analysis
- Scatterplots with linear trend lines
- Pearson correlation coefficients
- Coefficients of determination (R²)
- Year-over-year performance comparisons

## Preliminary Findings

### Section 1: Team Payroll and Regular-Season Performance

Team payroll demonstrated a weak-to-moderate positive relationship with regular-season wins and a negative relationship with losses.

- **Payroll vs. wins:** R² = 0.1167 (11.67% of variance explained)
- **Payroll vs. losses:** R² = 0.1177 (11.77% of variance explained)

These results suggest that team payroll alone is a relatively weak predictor of regular-season performance.

### Section 2: Year-Over-Year Payroll Changes and Team Performance

Changes in payroll demonstrated very weak relationships with changes in wins and losses.

- **Payroll change vs. win change:** r = -0.0759; R² = 0.00576 (0.58% of variance explained)
- **Payroll change vs. loss change:** r = 0.0781; R² = 0.00611 (0.61% of variance explained)

These findings suggest that increases in spending alone are not strongly associated with year-over-year improvements in team performance.

## Project Status

**In Progress**

### Completed
- [x] Initial data collection and preparation
- [x] Section 1: Payroll vs. Wins and Losses
- [x] Section 2: Changes in Payroll vs. Changes in Performance

### Planned
- [ ] Regression modelling
- [ ] Model diagnostics and validation
- [ ] Payroll efficiency comparisons
- [ ] Milwaukee Brewers case study
- [ ] Final discussion and conclusions

## Tools and Technologies

- **R** — Statistical analysis
- **RStudio** — Development environment
- **dplyr** — Data manipulation
- **ggplot2** — Data visualization
- **readxl** — Excel data import
- **R Markdown** — Reproducible reporting

## Limitations

This analysis is observational and does not establish a causal relationship between payroll and team performance. Factors such as player development, injuries, roster construction, and organizational decisions may also influence results. The pooled analysis additionally contains repeated observations of the same franchises across seasons.

## Future Directions

Future analysis will focus on developing regression models to estimate expected wins based on payroll, evaluating model performance, and identifying teams that outperform or underperform payroll-based expectations. The 2026 Milwaukee Brewers will serve as a featured case study.
  
