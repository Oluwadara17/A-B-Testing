## Title: A/B Testing
# Author: Oluwadara Olamide 

## Project Title
Fast Food Marketing Campaign A/B Test Analysis

## Introduction
This project analyses an **A/B marketing experiment** conducted by a fast-food chain planning to introduce a new menu item. The business tested **three different marketing promotions** across multiple store locations to determine which campaign generated the highest sales impact.

The analysis was completed as part of a graded task using the **Fast Food Marketing Campaign A/B Test dataset**, available in the `turing_data_analytics.wa_marketing_campaign` table.

## Objective

The primary goal of this analysis is to:

* Evaluate the performance of three marketing promotions.
* Apply appropriate **A/B testing and statistical inference techniques**.
* Identify the most effective marketing strategy.
* Provide **data-driven, actionable recommendations** to stakeholders.

## Dataset Overview
The dataset consists of **546 rows and 7 columns**, aggregated by location, promotion, and week.

### Columns

* **MarketID** – Unique identifier for the market
* **MarketSize** – Size of the market area by sales
* **LocationID** – Unique identifier for store location
* **AgeOfStore** – Store age in years
* **Promotion** – Marketing promotion (1, 2, or 3)
* **Week** – One of four weeks the promotion was run
* **SalesInThousands** – Weekly sales amount
  
## Tools & Technologies

* **Google BigQuery** – Data aggregation and preparation
* **Statistical Testing** – Pairwise t-tests with Bonferroni correction
* **Documentation** – All SQL and analysis stored in **`module 3 sprint 4.docx`**

## Analytical Approach

### Data Preparation

* The dataset was **aggregated by LocationID and Promotion** prior to statistical testing, as required.
* Weekly sales were summed per location to avoid repeated-measures bias.

### A/B Testing Strategy

* Since **three promotions** were tested, **pairwise comparisons** were conducted:

  * Promotion 1 vs Promotion 2
  * Promotion 1 vs Promotion 3
  * Promotion 2 vs Promotion 3

### Statistical Considerations

* A **99% confidence level** was used instead of 95% to reduce the risk of **Type I errors**.
* **Bonferroni correction** was applied to account for multiple comparisons:
[
\alpha_{adjusted} = 0.01 / 3 = 0.0033
]

## Aggregated Results

| Promotion | Avg Sales | Std Dev | No. of Locations |
| --------- | --------- | ------- | ---------------- |
| 1         | 232.40    | 64.11   | 43               |
| 2         | 189.32    | 57.99   | 47               |
| 3         | 221.46    | 65.54   | 47               |

## Statistical Test Results

### Promotion 1 vs Promotion 2

* **t-statistic:** 3.33
* **p-value:** 0.00128

✅ Statistically significant difference
➡ Promotion 1 performs better than Promotion 2.


### Promotion 1 vs Promotion 3

* **t-statistic:** 0.80
* **p-value:** 0.426

❌ No statistically significant difference detected.

### Promotion 2 vs Promotion 3

* **t-statistic:** −2.52
* **p-value:** 0.0136

❌ No statistically significant difference detected at the adjusted significance level.

## Conclusion

* **Promotion 1 significantly outperforms Promotion 2** in terms of average sales.
* There is **no statistically significant difference** between:

  * Promotion 1 and Promotion 3
  * Promotion 2 and Promotion 3

## Recommendation

Based on the statistical evidence:

* **Promotion 1** should be prioritised as the primary marketing strategy.
* The business should consider **continuing or expanding Promotion 1** to maximise sales performance.
* Further experimentation could be conducted to differentiate Promotion 1 and Promotion 3 more clearly.

## Appendix

All SQL queries used for data aggregation and preparation are documented in **Appendix 1** of the file: **`module 3 sprint 4.docx`**
