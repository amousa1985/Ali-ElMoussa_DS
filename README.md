A data science project focused on US crime rate analysis and prediction using historical data from 1960-2014.


Source: US crime rates from 1960–2014


Data cleaning – loads CSV, checks for nulls, removes outliers via z-score threshold

Trend visualization – plots crime category trends over time with matplotlib

Correlation heatmap – seaborn heatmap showing correlations between crime types

Anomaly detection – z-score-based anomaly detection (no anomalies found >3σ)

Key Observations

Crime peaked around 1990-1991 and generally declined through 2014
The "prediction" method is simple linear extrapolation, not a machine learning model
Predictions show declining crime rates for future years
The alert mechanism flags categories where predicted values exceed historical averages

