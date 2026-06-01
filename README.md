
Overview
A data science project focused on US crime rate analysis and prediction using historical data from 1960-2014.

Repository Structure
File	Description
Crime prediction.ipynb	Jupyter notebook with full analysis
US_Crime_Rates_1960_2014.csv	Dataset (55 rows, 12 columns)
Ali ElMoussa_DS.pptx	PowerPoint (presentation)
Data Summary
Source: US crime rates from 1960–2014
Features: Year, Population, Total crimes, Violent, Property, Murder, Forcible Rape, Robbery, Aggravated assault, Burglary, Larceny/Theft, Vehicle Theft
No missing values in the dataset
Notebook Workflow (5 cells)
Data cleaning – loads CSV, checks for nulls, removes outliers via z-score threshold
Trend visualization – plots crime category trends over time with matplotlib
Correlation heatmap – seaborn heatmap showing correlations between crime types
Anomaly detection – z-score-based anomaly detection (no anomalies found >3σ)
Crime prediction – uses scipy.interpolate.interp1d for linear extrapolation to predict future crime rates (2015–2018), with an alert system flagging categories above historical average
Key Observations
Crime peaked around 1990-1991 and generally declined through 2014
The "prediction" method is simple linear extrapolation, not a machine learning model
Predictions show declining crime rates for future years
The alert mechanism flags categories where predicted values exceed historical averages

