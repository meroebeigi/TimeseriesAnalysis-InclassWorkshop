# AirPassengers: Power BI analysis

[Open the interactive Power BI report](https://app.powerbi.com/groups/1dab85b5-c696-42fa-968e-e7c235d246d0/reports/7599d9ce-23e5-4a92-94bb-cd67811139b4)

The report is hosted in Power BI and may require sign-in and permission from its owner. This link does not grant access or publish the report publicly. A local Power BI export is available as [AirPassengers.pbix](AirPassengers.pbix). Download it and open it in Power BI Desktop.

## Report pages

- **Monthly trend:** passenger values over January 1949–December 1960.
- **Annual totals:** summed monthly values for each year.
- **Seasonality:** average values for each calendar month across all 12 years.

## Main findings

| Metric | Value |
|---|---:|
| Monthly observations | 144 |
| Annual total in 1949 | 1,520 |
| Annual total in 1960 | 5,714 |
| Annual-total compound growth, 1949–1960 | 12.8% |
| Annual growth in 1960 | 11.2% |
| Highest observation | July 1960: 622 |
| Lowest observation | November 1949: 104 |

July and August have the highest calendar-month averages; November has the lowest. The series combines a rising long-term trend with recurring seasonal peaks.

Values retain the CSV's original scale. The CSV headers do not state a unit multiplier.

## Data and calculations

Source: [AirPassengers.csv](AirPassengers.csv). The source contains 144 unique, consecutive monthly observations.

- Annual total = sum of the 12 monthly values in that year.
- Calendar-month average = sum of that month's observations divided by 12.
- Compound annual growth = (5,714 / 1,520)^(1/11) - 1.
- 1960 annual growth = 5,714 / 5,140 - 1.

The report was created from a static import of the supplied CSV. **Automatic refresh is not configured**, as requested. Changes to this repository's CSV will not automatically update the hosted report.

The repository's existing [time-series notebook](AirPassengers_TimeSeries_Portfolio.ipynb) contains the separate notebook analysis.
