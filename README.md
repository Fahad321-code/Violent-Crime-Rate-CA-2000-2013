# Violent Crime Analysis in California (2000-2013)

# Overview.

This research examines violent crime patterns in California counties and MPO regions from 2000 to 2013. The purpose was to investigate changes over time, geographical patterns, and estimate future crime trends using Python-based data science algorithms.

# Data Preprocessing.

Source: Raw violent crime data from the California government (https://catalog.data.gov/dataset/violent-crime-rate-9a68e/resource/e5df4a79-6b42-4f5e-83c7-8069dd943f4d)

# Cleaning Steps:

Removed missing and inconsistent values.

Standardized column names.

Verified data types and adjusted date formatting.

# Output: Cleaned dataset saved in data/cleaned_crime_data.csv.

# Exploratory Data Analysis (EDA).

# Summary statistics:

Descriptive statistics calculated for crime rate, count, and population.

# Visuals:

Crime rates have typically decreased between 2000 and 2013.

Crime Rate Distribution by Year: Displayed with box plots and scatter overlays.

Top Crime Types: Identified and classified according to average rate and count

Correlation Matrix: Shows correlations between numerical variables.

# Predictive modeling (Prophet)

Model: Facebook Prophet time series forecast.

# Input Features:

Report year: Year of observation.

rate (number of violent crimes per thousand population)

# Output:

Forecast of crime rate until 2018

Confidence intervals visualized

# Insight: Predicted crime rates continued to decline beyond 2013

# Geographic Analysis.

Regional Trends By MPO Region:

Total offenses Over Time: A line map of cumulative offenses by MPO region.

Average crime rate throughout time: regional comparisons using interactive and static charts.

# Interactive visuals:

# Choropleth Map: County-level crime rates are shown geographically.

Animated Timeline: Yearly Changes in Crime Rates by Region

Stacked Area Plot: Crime Trends over Time by Type (e.g., assault, robbery).

# Urban-Rural Comparison:

Classified counties using geotype and region_name.

Compared total violent crimes with average crime rates.

Urban counties had more total offenses, but some rural counties had higher per capita rates.

# outputs

Cleaned dataset: cleaned_crime_data.csv.

# Interactive HTML files:

violent_crime_choropleth_map.html

urban_rural_avg_rate.html

crime_timeline_animation.html

Notebooks: /notebooks/ directory

# Tools and Libraries

Python: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Folium, Prophet, GeoPandas.

Google Colab for Code Execution

GitHub for version control.

# Conclusion.

From 2000 to 2013, violent crime in California decreased consistently, according to the data. Regional inequities persist, with urban areas continuing to bear the brunt of occurrences. Time-series modeling supports the downward trend in crime rates, however geospatial representations highlight concentration locations.

Author: Independent Researcher (2025).Project repository: [GitHub link here]
