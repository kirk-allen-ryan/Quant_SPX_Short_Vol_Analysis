# Technical Summary: Quantitative Risk & Multi-Dimensional Modeling

## Executive Summary
This project establishes a systematic framework for analyzing high-dimensional datasets to optimize risk-adjusted returns. By engineering custom metrics and leveraging advanced visualization techniques, the pipeline identifies "efficiency frontiers" within a dataset of 40,000+ observations. The core logic focuses on **Extrinsic Value (EV)** optimization and the statistical normalization of variables across time-series and categorical bins.

## Core Data Engineering
* **Vectorized Permutation Engine:** Designed a dynamic lookup system in Excel to calculate 20-step risk scenarios across 5,500+ strike/date combinations.
<img width="928" height="434" alt="image" src="https://github.com/user-attachments/assets/7c40f274-1810-4ab3-9d56-cc1ceabd9322" />

* **Defensive Pipeline Design:** Implemented an automated Python ingestion script that enforces strict type-coercion, handles unit-conversion anomalies, and filters for high-integrity data points.
* **Feature Engineering:** Derived secondary metrics such as **TV_per_Unit (Efficiency)** and **Risk-Normalized Theta** to create a standard scale for comparing disparate data segments.

## Statistical & Visual Analysis
* **Non-Parametric Stratification:** Utilized **Boxen Plots** to visualize distribution density and "fat tails" without the skewing effect of outliers, ensuring conclusions are based on median-case reliability rather than anomalies.
* **Multi-Dimensional Heatmapping:** Developed pivot-based heatmaps to observe the intersection of three variables (e.g., Time Decay vs. Price Distance vs. Efficiency), enabling rapid identification of high-value clusters.
<img width="810" height="540" alt="image" src="https://github.com/user-attachments/assets/24a8766a-678d-4c55-9914-31e74b03646e" />

  
* **Lowess Smoothing & Convexity:** Applied **Locally Weighted Scatterplot Smoothing** to identify non-linear trends and curvature (convexity) within the data, moving beyond simple linear regressions to capture real-world behavior.

## Technical Stack
* **Python:** Pandas, NumPy, Seaborn, Matplotlib, Statsmodels.
* **Advanced Excel:** Dynamic Arrays, Lambda Functions, Matrix Lookups.
* **Methodology:** Risk Stratification, Efficiency Normalization, and Longitudinal Trend Analysis.

## Gallery

---

<img width="1385" height="905" alt="image" src="https://github.com/user-attachments/assets/e65e4dc8-6d51-4607-8017-9b03627f3bce" />

---

---

<img width="3145" height="2185" alt="image" src="https://github.com/user-attachments/assets/6dd02c29-8365-4a73-82e5-404230c8b03a" />

---

---

<img width="5919" height="2077" alt="image" src="https://github.com/user-attachments/assets/dd54a0b9-6b15-4c15-8de0-91c83f21f064" />

---

---

<img width="5551" height="1994" alt="image" src="https://github.com/user-attachments/assets/839c4b67-9856-470d-a350-352e38cf0434" />

---
