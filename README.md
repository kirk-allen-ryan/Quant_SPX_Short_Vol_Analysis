Quantitative Risk & Volatility Analysis (SPX)
[Clinical Analyst / Data Scientist Perspective]
🏗️ Project Overview
This repository contains a quantitative analysis of S&P 500 (SPX) short volatility spreads. The project demonstrates the ability to ingest large-scale raw data, perform feature engineering, and develop multi-dimensional visualizations to identify "optimal" risk-adjusted opportunities.

Clinical Relevance: The logic used here to find the "best time value per unit of risk" is mathematically analogous to identifying the most effective clinical intervention (Time Value) relative to patient risk profiles (Width/Moneyness).

🛠️ Technical Competencies & Clinical Parallels
1. Robust Data Preprocessing & Normalization
Technique: Automated ingestion of .xlsx/.csv formats with defensive "type-coercion" and handling of missing values (e.g., filtering out zero extrinsic values).

Clinical Application: Equivalent to cleaning Electronic Health Record (EHR) data, where handling inconsistent units (e.g., labs in mg/dL vs mmol/L) and removing physiological outliers is critical for model integrity.

2. Dimensionality Reduction & Binning
Technique: Engineered moneyness_bin categories (0.5% increments) and StepNum variables to transform continuous market data into actionable discrete buckets.

Clinical Application: Direct parallel to Patient Risk Stratification. Instead of "Moneyness," this logic is applied to stratifying patients by BMI, age cohorts, or lab value ranges to predict hospital readmission rates.

3. Quantitative Risk Metrics (The "TV_per_Unit" Logic)
Technique: Developed a custom efficiency metric: Time Value per Unit of Width. This measures the "yield" generated per unit of risk taken.

Clinical Application: Analogous to Cost-Effectiveness Analysis (CEA) or Number Needed to Treat (NNT). It quantifies the clinical "yield" (outcomes) against the "cost" (risk of adverse events or financial spend).

4. Advanced Data Visualization (Seaborn/Matplotlib)
Heatmaps: Visualizing Average Extrinsic value across DTE (Days to Expiration) and Moneyness.

Healthcare Use: Mapping disease prevalence or resource utilization across time and demographic segments.

Boxen/Box Plots: Using non-parametric distributions to compare "Calls vs Puts" efficiency while hiding extreme outliers.

Healthcare Use: Comparing treatment efficacy across different patient cohorts (e.g., Drug A vs. Drug B) while accounting for high-variance clinical outcomes.

LOWESS Smoothing: Implementing locally weighted scatterplot smoothing to identify non-linear trends (convexity) in time-decay.

Healthcare Use: Analyzing longitudinal patient data, such as glucose monitoring trends or medication adherence patterns over time.

🧪 Statistical Methods Used
Pivot Tables & Aggregations: Aggregating 40,000+ rows into mean/median grids.

Non-Parametric Analysis: Using medians and IQR (via Boxen plots) to ensure findings are not skewed by market anomalies.

Risk-Normalization: Calculating "Risk-normalized theta" by dividing time-decay by Delta absolute values.

🚀 Impact Statement
This project showcases the ability to take a complex, high-frequency dataset and distill it into a strategic "decision support" tool. Whether the "Risk" is financial loss or patient morbidity, the analytical framework—Ingest → Clean → Bin → Metricize → Visualize—remains the gold standard for data-driven decision making.
