# Analyzing Maternal Mortality Disparities: Statistical Insights and Public Health Challenges

Why does the country with one of the world's highest Human Development
Index scores also have the worst maternal mortality rate in the developed
world — and who bears that burden?

See the [data dashboard](./maternal-mortality-dashboard.pdf) (built in
Tableau) for a visual summary, or the [full white paper](./maternal-mortality-report.docx)
for the complete analysis and discussion.

**Team project** — completed with Peterson Le and Juliette Oliver for
Digital Humanities 150: Data Analysis for Social Research, UCLA (Dr.
Ashley Sanders). Contributed across all parts of the analysis: the ANOVA
testing, the contingency tables, and the country-level five-number
summary.

## Overview

The U.S. ranks highly on the Human Development Index yet has the highest
maternal mortality rate (MMR) among developed nations. This project
investigates two questions: why does that gap exist, and which
populations are disproportionately affected? Using OECD country-level
data and CDC race-specific data on pregnancy-related deaths, the analysis
tests whether racial disparities — not just overall healthcare quality —
help explain the U.S.'s outlier status.

## Approach

- **ANOVA test**: compared maternal mortality rates across White, Black,
  and Hispanic women for all causes of pregnancy-related death, testing
  whether race is associated with a statistically significant difference
  in MMR.
- **Contingency tables & bar charts**: analyzed CDC data (2006–2017) on
  the number and type of pregnancy-related deaths to identify leading
  causes of death and how they break down by race.
- **Five-number summary**: compared 2018 OECD maternal mortality data
  across developed countries with up-to-date reporting, positioning the
  U.S. against international peers.
- **Tools**: R (`ggplot2`, `plotly`, R Markdown) for statistical analysis
  and visualization, Google Sheets for collaborative data cleaning across
  the team, Tableau for the final dashboard.

## Key findings

- **Race is a statistically significant factor**: the ANOVA test returned
  p < .05, rejecting the null hypothesis that there's no racial
  difference in maternal mortality rates.
- **The U.S. is a clear outlier internationally**: a 2018 MMR of 17.40
  deaths per 100,000 live births — more than 4x the dataset's median of
  4.30 (Sweden), and well above the upper quartile (Korea, 11.3). Only
  Mexico's 34.6 was higher, treated as a separate outlier given its very
  different HDI/GDP profile.
- **The U.S. rate has been rising, not falling**: from 14.5 (2000) to
  17.2 per 100,000 live births (2015), with no sign of reversal.
- **Racial disparity in outcomes is stark**: Black and American Indian
  women showed substantially higher pregnancy-related mortality per
  100,000 live births than Asian, White, or Hispanic women in the CDC
  data — and Black women also showed markedly higher rates of death from
  anesthesia complications specifically, a pattern the paper connects to
  documented disparities in hospital quality by neighborhood
  demographics.
- **Most of these deaths are preventable**: cardiovascular causes
  (cardiomyopathy, thrombotic pulmonary conditions, hypertensive
  disorders, and other cardiovascular disease) account for a large share
  of pregnancy-related deaths — conditions that are generally treatable
  with adequate, timely care.

## Repository structure

```
├── maternal-mortality-report.docx    # full write-up: methods, statistical tests, discussion
├── maternal-mortality-dashboard.pdf       # Tableau dashboard summarizing key statistics
└── README.md
```

## Tools

R · ggplot2 · plotly · R Markdown · Google Sheets (collaborative
cleaning) · Tableau (dashboard) · ANOVA · contingency table analysis ·
five-number summary

## Data sources

- CDC, National Center for Health Statistics — Compressed Mortality File
- Organization for Economic Co-operation and Development (OECD) —
  2018 country-level maternal mortality reports
- MacDorman, M. F., Declercq, E., & Thoma, M. E. (2017). Trends in
  Maternal Mortality by Sociodemographic Characteristics and Cause of
  Death. *Obstetrics and Gynecology, 129*(5), 811–818.

## Author

Anna Gutierrez, with Peterson Le and Juliette Oliver —
[portfolio](https://annagtz1.github.io) · [LinkedIn](https://www.linkedin.com/in/anna-gutierrez-m-s/)
