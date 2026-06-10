# NHS RTT Waiting Times Dashboard

An interactive Power BI dashboard analysing NHS Referral to Treatment (RTT) waiting times across England from January 2021 to March 2025. Built as a portfolio project to demonstrate Power BI, DAX, and healthcare data analysis skills.

<img width="1348" height="753" alt="dashboard" src="https://github.com/user-attachments/assets/47fde200-7c00-4449-9cd4-5dc0f64c94e3" />

---

## Overview

The NHS waiting list crisis has been one of the most significant pressures on the health service since the Covid pandemic. This dashboard tracks the growth of the waiting list from January 2021 through to March 2025, surfacing key metrics around volume, year on year change, and the proportion of patients waiting beyond critical thresholds.

---

## Features

### KPI Cards

Five cards across the top of the Summary page provide an at a glance snapshot of the current state of the waiting list:

| Card | Description |
|------|-------------|
| Patients waiting right now | Total patients on the waiting list at the latest selected date |
| Average monthly patients waiting | Mean monthly waiting list size across the selected date range |
| Change vs same month last year | Year on year change in waiting list size with conditional formatting (red for increase) |
| Waiting over 52 weeks | Total patients waiting beyond 52 weeks at the latest date |
| % Over 52 Weeks | Proportion of the waiting list that has been waiting over 52 weeks |

### Charts

**Monthly waiting list trend**
Line chart showing total waiting list size by pathway type from January 2021 to March 2025. Includes a Pre-Covid baseline reference line at 10 million patients, providing context for how far the waiting list has grown beyond pre-pandemic levels.

**Top 5 specialties by wait list**
Horizontal bar chart showing the five specialties with the largest waiting lists, filtered to the selected date range and pathway type.

**Top 5 specialties by long waiters (52+ weeks)**
Horizontal bar chart showing the five specialties with the highest number of patients waiting beyond 52 weeks.

### Slicers

Three slicers are synced across both pages:

- Archive Date (date range slider)
- Pathway Type (dropdown)
- Specialty (dropdown)

---

## Data Model

- **Source table:** NHS_2021_2025_master containing monthly RTT data by specialty and pathway type
- **Date table:** Rebuilt as a DAX calculated table spanning January 2021 to March 2025, related to Archive_Date in the master table
- **Key measures:** Total Wait List, Latest Month Wait List, Avg Wait List, Long Waiters 52wks, YoY Change, YoY Color (drives conditional formatting), % Over 52 Weeks

---

## Data Source

**Dataset:** NHS Consultant-Led RTT Waiting Times (2021 to 2025)

**Source:** Kaggle, published by hammad9191

**URL:** https://www.kaggle.com/datasets/hammad9191/nhs-consultant-led-rtt-waiting-times20212025

**Coverage:** January 2021 to March 2025

The dataset is derived from NHS England Referral to Treatment (RTT) Waiting Times Statistics and records the number of patients on incomplete pathways by specialty and pathway type each month at a national level.

---

## Tools Used

- Power BI Desktop
- DAX
- Power Query

---

## Project Status

The Summary page is complete and published. A Detail page with a specialty level breakdown matrix is currently in development and will be published in a future iteration.

---

## Author

**Mahanoor Shams**
[linkedin.com/in/mahanoor-shams](https://linkedin.com/in/mahanoor-shams)
[github.com/mayasyed](https://github.com/mayasyed)
