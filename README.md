# Co-occurring Mental Illness and Substance Use Disorders (NSDUH 2021–2024)

This repository hosts the interactive Plotly visualizations for a CSE 163
final project analyzing co-occurring any mental illness (AMI) and substance
use disorders (SUD) among U.S. adults, using the combined 2021–2024 National
Survey on Drug Use and Health (NSDUH) public use file.

**Author:** Steven Shi

## Viewing the Visualizations

The interactive charts are hosted with GitHub Pages. Once Pages is enabled,
each chart can be opened in a browser at:

```
https://sbeveshi.github.io/NSDUH-project/<filename>.html
```

For example:
`https://sbeveshi.github.io/NSDUH-project/rq3_forest.html`

## Research Questions and Charts

### RQ1 — How do rates of AMI, SUD, and co-occurrence vary across demographic groups?

Grouped bar charts showing the weighted percentage of adults in each
co-occurrence category (SUD only, AMI only, both, neither) by demographic.

- `rq1_IRSEX.html` — by sex
- `rq1_NEWRACE2.html` — by race/ethnicity
- `rq1_IRPINC3.html` — by income
- `rq1_IREDUHIGHST2.html` — by education
- `rq1_IRINSUR4.html` — by insurance status
- `rq1_COUTYP4.html` — by county type (urbanicity)

### RQ2 — Did the co-occurrence rate change between 2021 and 2024, and what drove it?

- `rq2_trend.html` — annual co-occurrence rate, 2021–2024
- `rq2_substance_trend.html` — annual alcohol use and illicit drug use rates

### RQ3 — What proportion of co-occurring adults receive treatment, and how does it vary?

Treatment receipt is limited to 2022–2023, the only years treatment data
was collected.

- `rq3_IRSEX.html` — treatment rate by sex
- `rq3_NEWRACE2.html` — treatment rate by race/ethnicity
- `rq3_IRPINC3.html` — treatment rate by income
- `rq3_IREDUHIGHST2.html` — treatment rate by education
- `rq3_IRINSUR4.html` — treatment rate by insurance status
- `rq3_COUTYP4.html` — treatment rate by county type
- `rq3_forest.html` — logistic regression odds ratios with 95% confidence
  intervals

### RQ4 — Among untreated co-occurring adults, what were the most common barriers?

- `rq4_barriers.html` — overall ranking of reported treatment barriers
- `rq4_barriers_insurance.html` — barriers broken down by insurance status

## Notes

- Visualizations use survey weights (`ANALWT2_C4` for 4-year analyses,
  `ANALWT2_C2` for the 2022–2023 treatment analyses) to produce
  population-representative estimates.
- The analysis code, testing module, and written report are submitted
  separately through Gradescope.

## Data Source

Substance Abuse and Mental Health Services Administration (SAMHSA),
combined 2021–2024 National Survey on Drug Use and Health (NSDUH) public
use file. Available from the SAMHSA Center for Behavioral Health Statistics
and Quality (CBHSQ) data portal.
