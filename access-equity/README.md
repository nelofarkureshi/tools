# Access & Equity Explorer: Primary and Specialist Care in Canada (2024)

An interactive tool for comparing primary and specialist care access across
Canadian provinces, built on Statistics Canada's 2024 Survey on Health Care
Access and Experiences (Primary and Specialist Care). Every estimate is shown
with its 95% confidence interval and tested against the national rate, and
results can be broken down by age group and gender.

The tool deliberately highlights which provincial differences are statistically
meaningful, rather than presenting rankings that overstate them.

**Live tool:** https://tools.nelofarkureshi.com/access-equity/

## What it does

- Choose any of 18 access, quality, cost, experience, and health-status indicators.
- Compare all ten provinces against the national rate, with significance marked.
- Stratify by gender (Men+ / Women+) and age group (18–44, 45–64, 65+).
- Read every estimate with its 95% confidence interval in a forest plot.
- Inspect within-population gaps (age gradient, gender gap) for any province.

## How it is built

A single self-contained HTML file. No server, no build step, no dependencies.
All published estimates are embedded directly in the page, so it can be hosted
as a static file anywhere (this copy runs on GitHub Pages).

## What it does and does not claim

The only formal test in the source is each province against the national rate
(bootstrapped, p < 0.05), uncorrected for multiple comparisons. Province-to-
province, age, and gender differences are shown with confidence intervals for
inspection but are not formally tested. The tool performs no additional
modelling; it re-presents published aggregate estimates.

## Data source and licence

Statistics Canada, Table 13-10-0962-01, Survey on Health Care Access and
Experiences (Primary and Specialist Care), 2024. Reproduced and distributed on
an "as is" basis with the permission of Statistics Canada.

Gender categories (Men+, Women+) are a modified two-category gender variable,
not sex; non-binary respondents are redistributed under Statistics Canada
confidentiality rules. Territories are excluded.

## Author

Built by Nelofar Kureshi. https://nelofarkureshi.com

Free to share and reuse with attribution.
