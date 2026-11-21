# Supermarket Sales Analysis Dashboard

An interactive Power BI report that tracks supermarket sales over time and compares performance by branch, product line, customer segment, and payment method. The dataset contains 1,000 transactions across Yangon, Mandalay, and Naypyitaw from January to March 2019.

## Sales snapshot

| Metric | Result |
| --- | ---: |
| Transactions | 1,000 |
| Units sold | 5,510 |
| Total sales including tax | 322,966.75 |
| Gross income as recorded in the source | 15,379.37 |

The source’s `gross income` field equals its `Tax 5%` field for every transaction. The report displays the supplied metric under its original name.

## Findings

- **Branch performance.** Naypyitaw had the highest total sales at 110,568.71.
- **Product performance.** Food and beverages led by sales value at 56,144.84. Electronic accessories led by units sold at 971.
- **Sales timing.** Saturday and Tuesday led in total sales across the period, while Monday ranked lowest. This pattern can inform when to test promotions and review staffing needs.

## Data preparation and reporting

- Prepared the source in Excel as a transaction table and two lookup sheets. `Fact Market` stores transaction measures, `Dim Branch` maps the three cities to branch codes, and `Dim Product` maps invoice IDs to product lines.
- Built a Power BI overview with KPI cards and sales breakdowns. The detail view compares sales by weekday and hour, and slicers support comparisons by year, month, city, product line, and payment method.
- Summarized findings and potential retail actions on the **Insights & Recommendation** page.

## Open the project

1. Download the [Power BI report](dashboard/Supermarket%20Sales%20Dashboard.pbix) and open it in Power BI Desktop for Windows.
2. Download the [prepared Excel workbook](data/CleanedData.xlsx) to inspect the model inputs. If Power BI prompts for a source when refreshing, update the file path in **Transform data → Data source settings** to point to your local copy.

## Data source

The data comes from Salah Sammari’s [Supermarket Sales Analysis with Data Science dataset on Kaggle](https://www.kaggle.com/datasets/midouazerty/supermarket-sales-analysis-with-data-science). The accompanying [analysis notebook](https://www.kaggle.com/code/midouazerty/supermarket-sales-analysis-advanced-level/notebook) is credited in the original project notes. The raw `market.csv` is available on the dataset page.
