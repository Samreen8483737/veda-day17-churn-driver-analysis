# Day 17: Churn Driver Analysis

## Objective
Develop a structured churn investigation using a Telco dataset to find customer attributes strongly associated with churn, ensuring all findings avoid unsupported causal claims.

## Technical Implementation
Utilized Python and Pandas to analyze categorical variables and calculate churn density across different customer segments.

1. **Segment Analysis:** Grouped data by key attributes (`Contract` and `TechSupport`) and calculated the mean churn rate (expressed as a percentage) within each specific cohort.
2. **Driver Ranking:** Quantified the impact of each attribute by measuring the "spread" (the difference between the highest and lowest churn rates within a category).
   * **Contract Type** emerged as the primary driver (29.11% spread between Month-to-month and Two-year contracts).
   * **Tech Support** emerged as a secondary driver (17.44% spread between having support and not having it).

## Recommendations & Findings
* **Finding:** Customers on Month-to-month contracts exhibit a significantly higher association with churn (50.10%) compared to those on 1- or 2-year contracts. 
* **Finding:** The lack of Tech Support is also heavily associated with higher churn (44.40%). 
* **Analytical Note:** These correlations do not definitively prove causation; however, they identify high-risk segments.
* **Recommendation:** Business teams should explore incentivizing Month-to-month customers to switch to annual plans (e.g., through targeted discounts) and proactively offer Tech Support to new sign-ups to potentially mitigate these high-risk associations.
