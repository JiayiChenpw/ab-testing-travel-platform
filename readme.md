# A/B Testing Analysis: Travel Platform Search Algorithm Optimization

## About the Project

This project analyzes the effectiveness of a new search ranking algorithm for an online travel platform. The experiment evaluates whether the algorithm improves conversion rates without negatively impacting user experience. The analysis demonstrates comprehensive A/B testing methodology from experimental design to business impact assessment.

**Business Question**: Should we deploy a new search algorithm that could improve booking conversions?

**Answer**: Yes - deploy based on statistically significant 14.22% conversion improvement and $2.1M projected annual revenue impact.

## Key Findings

**Primary Results**
* Conversion Rate Improvement: +2.27 percentage points (15.92% → 18.19%)
* Statistical Significance: p < 0.001 
* User Experience: No negative impact on booking time
* Annual Revenue Impact: $2.1M additional revenue projected

**Strategic Insights**
* Returning users benefit most: 16.5% relative improvement (highly significant)
* New users show positive trends: 9.8% improvement 
* Consistent performance across weekdays and weekends

## Technical Methodology

**Statistical Techniques**
* Sample Ratio Mismatch testing for randomization validation
* Bootstrap validation for non-parametric confirmation
* Multiple testing correction using Bonferroni adjustment
* Statistical power analysis (96% power achieved)
* Effect size quantification with confidence intervals

**Analysis Framework**
* Primary Metric: Conversion rate using Z-test for proportions
* Guardrail Metrics: Time-to-booking using Welch's t-test
* Segmentation Analysis: User type and temporal patterns
* Assumption Validation: Normality testing with Central Limit Theorem
* Business Impact: Revenue modeling with confidence intervals


**Data Requirements**

The analysis expects two CSV files with the following structure:
* `sessions_data.csv`: Session-level data with timestamps, user IDs, and booking outcomes
* `users_data.csv`: User-experiment group assignments for A/B test participants

Note: Original datasets are not included due to data privacy considerations.

## Results Summary

| Metric | Control | Variant | Improvement | Significance |
|--------|---------|---------|-------------|--------------|
| Conversion Rate | 15.92% | 18.19% | +14.22% | p < 0.001 |
| Time to Booking | 15.01 min | 14.89 min | -0.79% | p = 0.54 |
| Daily Sessions | 7,630 | 7,653 | Balanced | p = 0.86 |

## Skills Demonstrated

* Experimental Design and A/B test validation
* Advanced statistical analysis and hypothesis testing
* Business impact modeling and ROI quantification

## Data Source

This analysis is based on the DataCamp A/B Testing Dataset, providing a realistic travel platform scenario.

**Related Certification**: [Customer Analytics and A/B Testing in Python](https://www.datacamp.com/completed/statement-of-accomplishment/course/c657518a9edd804103d30328fccbc92494991e70)