# Meta DTC Swimwear Ads Q1 Analysis & Creative A/B Test
Python Portfolio Project | Pandas, Matplotlib, Two-proportion Z-test

## Project Overview
This project performs a full quarterly review of Meta advertising data for a DTC swimwear brand, using anonymized Q1 (Jan-Mar) ad records.
The cleaned dataset contains 3,588 ad records and 40 business metrics.
Three core analysis modules:
1. Multi-dimensional performance review: Break down ROAS, Spend, and GMV across time, country, and creative dimensions to identify high-value markets and inefficient ad groups.
2. User conversion funnel: Build a 6-stage logarithmic scale funnel to locate the biggest drop-off point from impression to final purchase.
3. Creative A/B significance test: Use a two-proportion Z-test to compare the CTR of video vs. static creatives, distinguishing real performance differences from random fluctuations.

## Tech Stack
Python | Pandas | Matplotlib | NumPy | SciPy
- Data cleaning: Deduplication, filtering abnormal samples, handling missing values, and computing derived metrics (ROAS, CTR, conversion rates).
- Visualization: Customized conversion funnel chart, market ROAS comparison, and creative CTR bar chart with 95% confidence intervals and proper layout spacing.
- Statistics: Two-proportion Z-test to verify CTR difference statistical significance.

## Key Findings
1. Market performance: Australia delivers the top ROAS. Germany exhibits higher ad spend inefficiency, though all major markets maintain positive ROAS above break-even.
2. Conversion bottleneck: The sharpest user drop occurs at the Landing Page → Add-to-Cart stage, with a conversion rate of only 9.69%. This represents the core optimization target.
3. Creative insight: Video creatives achieved a CTR of 2.250% compared to 2.151% for static images, showing a statistically significant difference ($p < 0.05$) in favor of video.

## Business Recommendations
✅ Shift additional budget to Australia to scale profitable returns.
✅ Pause or iterate low-performing ad sets in Germany to minimize wasted spend.
✅ Prioritize video creatives for upcoming campaigns while scaling down static ad proportions.
✅ Optimize product detail pages, size guides, and user-generated content to improve Landing-Page-to-ATC conversion.

## Project Limitation
This A/B analysis is a retrospective observational study rather than an official online randomized controlled experiment (RCT). Confounding variables such as audience allocation, budget fluctuations, and seasonality cannot be fully eliminated. The findings indicate strong correlation rather than strict causal effects. A formal randomized online experiment is recommended for final causal validation.

## File Description
- Meta_Ads_Swimwear_Q1_Analysis.ipynb: Full analysis notebook including code, visual adjustments, and detailed markdown explanations.
- To C meta ads Swimsuit Q1.xlsx: Anonymized raw advertising dataset.
