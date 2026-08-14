# Railway Data Engineering Report

## Dataset Summary

- Total Records: 11,113
- Total Unique Trains: 11,113
- Unique Source Stations: 921
- Unique Destination Stations: 924

## Station Insights

- Top Source Station: CST-MUMBAI (513 trains)
- Top Destination Station: CST-MUMBAI (514 trains)

## Day-wise Train Distribution

| Day | Trains |
|---|---:|
| Friday | 1,649 |
| Tuesday | 1,628 |
| Wednesday | 1,612 |
| Sunday | 1,602 |
| Saturday | 1,593 |
| Thursday | 1,526 |
| Monday | 1,503 |

## Weekday vs Weekend

| Category | Trains |
|---|---:|
| Weekday | 7,918 |
| Weekend | 3,195 |

## Route Analysis

**Most Frequent Route:** TAMBARAM → CHENNAI BEACH  
**Services:** 137

## Correlation Analysis

Correlation between day number and train count:

**0.3806**

## Key Insights

- Train operations are more concentrated on weekdays.
- CST-MUMBAI is a major railway hub.
- Several routes have high service frequency.
- Day-wise patterns can help with capacity planning.

## Business Recommendations

- Optimize scheduling at high-traffic stations.
- Use day-wise trends for capacity planning.
- Analyze high-frequency routes for service optimization.
- Evaluate weekend demand before increasing services.
- Focus infrastructure planning on major railway hubs.

## Executive Summary

This PySpark-based analysis processed railway operational data to identify major railway hubs, high-frequency routes, day-wise service patterns, and weekday versus weekend trends. The findings can support railway scheduling, capacity planning, and operational decision-making.