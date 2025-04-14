# Economy-Prediction
Data analysis on Maldives' economic growth prediction.

Use changes in nighttime lights and internet speeds to predict economic development, focusing on the interplay between digital infrastructure and economic activity.
Datasets:
1.	Ookla Speedtest Data:
o	Metrics: Download/upload speeds, latency, and test counts.
o	Spatial Coverage: Global, with ~610.8m × 610.8m tiles.
o	Temporal Coverage: Quarterly data from Q1 2019 to Q2 2024.
2.	VIIRS Annual Composites:
o	Metrics: Radiance values indicating human activity and economic infrastructure.
o	Spatial Coverage: Global, with ~500m resolution.
o	Temporal Coverage: Annual data from 2012 to 2021.

Procedural Details:

Data Preprocessing:
1.	VIIRS Data:
o	Extract annual radiance data at regional or national levels.
o	Calculate percentage changes in radiance over time to represent economic growth.
2.	Ookla Data:
o	Aggregate quarterly internet speed data into annual averages to align with VIIRS temporal granularity.
o	Focus on download speeds, as they are a key indicator of internet infrastructure performance.
3.	Integration:
o	Perform spatial joins to align Ookla tiles with VIIRS grids or administrative boundaries (e.g., countries or regions).
o	Create a unified dataset that includes radiance changes, internet speeds, and economic indicators (e.g., GDP growth, if available).

EDA and Visualizations:
1.	Heatmap:
o	Show regional variations in radiance intensity and internet speeds.
2.	Scatter Plot:
o	Correlate changes in radiance with internet speeds to identify trends.
3.	Bar Chart:
o	Compare regions with different levels of radiance growth and internet performance.
4.	Geospatial Overlay:
o	Map regions with high radiance growth and fast internet speeds to highlight economic hotspots.
5.	Line Chart:
o	Display time-series trends in radiance and internet speeds for key regions.

Hypothesis Testing:
•	Null Hypothesis: Changes in nighttime light intensity and internet speeds are not significantly associated with economic development.
•	Alternative Hypothesis: Changes in nighttime light intensity and internet speeds are significantly associated with economic development.

Prediction Model Objective:
•	Objective: Predict regional economic growth (e.g., GDP growth) using changes in nighttime light intensity and internet speeds as predictors.
