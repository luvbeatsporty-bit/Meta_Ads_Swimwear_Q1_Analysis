# Meta DTC Swimwear Ads Q1 Analysis & Creative A/B Test
Python Portfolio Project | Pandas, Matplotlib, Two-proportion Z-test

## Project Overview
This project performs a full quarterly review of Meta advertising data for a DTC swimwear brand, using anonymized Q1 (Jan-Mar) ad records.
The cleaned dataset contains 3588 ad records and 40 business metrics.
Three core analysis modules:
1. Multi-dimensional performance review: Break down ROAS, Spend and GMV from time, country and creative dimensions to identify high-value markets and low-efficiency ad groups.
2. User conversion funnel: Build a 6-stage funnel to locate the biggest drop-off point from impression to final purchase.
3. Creative A/B significance test: Use two-proportion Z-test to compare CTR of video vs static creatives, distinguish real performance difference from random fluctuation.

## Tech Stack
Python | Pandas | Matplotlib | NumPy | Scipy
- Data cleaning: Deduplication, filter abnormal samples, handle missing values, compute derived metrics (ROAS, CTR, conversion rates)
- Visualization: Daily trend chart, market ROAS comparison, conversion funnel, creative CTR bar chart
- Statistics: Two-proportion Z-test to verify CTR difference statistical significance

## Key Findings
1. Market performance: Australia delivers the best ROAS. Germany has wasted ad spend. All markets maintain positive ROAS above break-even point.
2. Conversion bottleneck: The largest user drop occurs at Landing Page → Add-to-Cart stage, conversion rate only 9.78%. This is the core optimization point.
3. Creative insight: Video creatives have statistically significantly higher CTR than static images (p<0.05).

## Business Recommendations
✅ Shift more budget to Australia to scale profitable returns
✅ Pause or iterate low-performing ad sets in Germany to reduce wasted spend
✅ Prioritize video creatives for new campaigns, reduce static creative proportion
✅ Optimize product page, size guide and buyer photos to improve Landing-Page to ATC conversion rate

## Project Limitation
This A/B analysis is a retrospective observation test instead of official online randomized A/B experiment. Confounding variables like audience, budget and time cannot be fully eliminated. Results show correlation instead of strict causal effect. Formal randomized online experiment is required for causal validation.

## File Description
- Meta_Ads_Swimwear_Q1_Analysis.ipynb: Full analysis notebook with markdown explanation, Python code and visualization
- To C meta ads Swimsuit Q1.xlsx: Anonymized raw advertising dataset
