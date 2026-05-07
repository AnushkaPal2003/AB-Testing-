# A/B Testing Analysis: Impact of New Landing Page on User Conversion (294K Sessions)

# A/B Testing for Landing Page Optimization
## Problem Statement


This project evaluates whether a new landing page improves user conversion compared to the existing page using A/B testing on ~290K user sessions.

The goal is to make a data-driven decision using statistical analysis.


## Goal
Provide **data-driven insights** to determine whether the **new landing page should replace the old page** based on statistical evidence.

The dataset contains:

- user_id: unique user identifier
- timestamp: session time
- group: control or treatment
- landing_page: old or new page
- converted: 1 if user converted, else 0

Total observations: ~294,000

# Experiment Design

Control group users saw the old landing page, and treatment group users saw the new landing page. Users were randomly assigned.

The objective was to compare conversion rates between the two groups.

# Metrics Used

Primary metric:Conversion Rate


Secondary metric:Daily conversion trend

Guardrail metrics (not available in data but important in real experiments):

Bounce rate
Page load time
Errors or crashes
Data Quality Check

A validation check was performed to ensure correct mapping between group and landing page.

Mismatch rows found: 3893

These rows were removed to maintain experiment integrity.

# Key Results

Overall conversion rate: ~11.96%

Group-wise conversion rates:

Control: ~12.04%
Treatment: ~11.88%

Group sizes were nearly equal, ensuring fair comparison.

# Statistical Test

A two-proportion Z-test was used.

Z-statistic: ~1.23
P-value: ~0.216

Significance level: 0.05

# Interpretation

Since the p-value is greater than 0.05, the result is not statistically significant. The difference in conversion rates is likely due to random variation.

# Final Decision

Do not launch the new landing page, as there is no statistically significant improvement in conversion rate.

# Limitations
No user segmentation analysis
No long-term retention measurement
No confidence intervals
Guardrail metrics not included
Possible external factors not controlled

# Conclusion

The analysis shows that the new landing page does not significantly improve conversion rates. Therefore, there is no strong evidence to support its launch.

