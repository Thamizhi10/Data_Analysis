# E-news Express — Landing Page A/B Test Analysis

## Problem Statement
E-news Express, an online news portal, has seen a decline in new monthly subscribers. The design team built a new landing page with an improved outline and more relevant content. As a data scientist, the task is to statistically evaluate whether the new landing page performs better than the existing one at driving subscriptions, using data from a randomized A/B test (50 users on the old page, 50 on the new page).

## Approach
Ran four hypothesis tests at a 5% significance level to answer the business questions:

1. **Time spent on page** — two-sample t-test comparing time spent on the new vs. old landing page
2. **Conversion rate** — two-proportion z-test comparing subscriber conversion rates between pages
3. **Conversion vs. language** — chi-square test of independence to check if conversion depends on preferred language
4. **Time spent across languages** — one-way ANOVA to test whether time spent on the new page differs by language group, with assumption checks (Shapiro-Wilk test for normality, Levene's test for homogeneity of variance) run before the ANOVA itself

## Key Findings
- Users spend significantly more time on the new landing page (p ≈ 0.0001)
- The new page has a significantly higher conversion rate (p ≈ 0.016)
- Conversion status is independent of preferred language (p ≈ 0.213)
- Time spent on the new page does not significantly differ across language groups (p ≈ 0.432)

## Skills
Hypothesis testing, A/B test design and interpretation, two-sample t-test, two-proportion z-test, chi-square test of independence, one-way ANOVA, test assumption validation (normality, homogeneity of variance)

## Tech Stack
Python, pandas, NumPy, Matplotlib, Seaborn, SciPy, statsmodels

## Dataset
E-news Express A/B test data (100 users, control/treatment groups), provided as part of PGP-AIML coursework.
