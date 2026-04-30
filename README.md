# San Francisco Airbnb Listing Performance Analysis

## Overview

This project analyzes San Francisco Airbnb listings to identify which listing, host, and neighborhood characteristics are associated with higher occupancy. The analysis focuses on occupancy as the main performance metric and aims to generate practical business insights for hosts.

## Business Question

Which listing and host features are associated with higher occupancy for Airbnb listings in San Francisco?

## Dataset

- Source: [Inside Airbnb](https://insideairbnb.com/get-the-data/)
- Local file used: `sf_listings.csv`

The dataset includes listing characteristics, host information, review activity, availability data, and estimated occupancy values.

## Tools Used

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Key Findings

1. Occupancy varies widely across San Francisco Airbnb listings, suggesting that listing performance is highly uneven across the market.

2. Room type and neighborhood are two of the clearest structural factors associated with occupancy. Entire homes generally outperform private rooms, while shared rooms should be interpreted cautiously because of their much smaller sample size.

3. Superhost status is one of the strongest and most consistent host-side signals in the analysis. Superhost listings show higher occupancy overall and continue to outperform when compared across neighborhoods and host acceptance-rate groups.

4. Host acceptance rate is positively associated with occupancy, suggesting that hosts who accept more booking requests may be better positioned for stronger listing performance.

5. Review activity, especially `number_of_reviews` and `reviews_per_month`, is strongly associated with higher occupancy, although these should be treated as performance-related signals rather than clear causal drivers.

6. Minimum-stay rules showed a meaningful pattern, with 2-night and 3–6-night stays generally associated with stronger occupancy than longer minimum-stay groups.

## Recommendations

1. Hosts should prioritize strong host-quality signals, especially **Superhost** status, booking acceptance behavior, and responsiveness.

2. Guest experience should be treated as a core growth lever, since stronger review activity is closely associated with higher occupancy.

3. Shorter minimum-stay policies may support stronger occupancy, especially 2-night and 3–6-night requirements, but they should still be evaluated within the listing’s room type and market segment.

4. Hosts should benchmark against comparable listings within the same room type and neighborhood rather than relying on broad citywide averages.

## Limitations

1. `price` and `estimated_revenue_l365d` were unavailable in this dataset extract, so the analysis focuses on occupancy rather than pricing or revenue.
2. `estimated_occupancy_l365d` is an estimated measure rather than direct booking data.
3. The analysis is observational, so findings should be interpreted as associations rather than causation.
4. Some categories, such as shared rooms, have much smaller sample sizes and should be interpreted cautiously.

## Conclusion

Occupancy in San Francisco appears to be most strongly associated with a combination of listing structure, neighborhood context, and host-quality signals. Among the host-side factors, **Superhost** status stands out as one of the most consistent indicators of stronger booking performance.
