# Violent Crime Analysis in California (2000-2013)

# Overview.

This research examines violent crime patterns in California counties and MPO regions from 2000 to 2013. The purpose was to investigate changes over time, geographical patterns, and estimate future crime trends using Python-based data science algorithms.

# Data Preprocessing.

Source: Raw violent crime data from the California government (https://catalog.data.gov/dataset/violent-crime-rate-9a68e/resource/e5df4a79-6b42-4f5e-83c7-8069dd943f4d)

# Cleaning Steps:

Removed missing and inconsistent values.

Standardized column names.

Verified data types and adjusted date formatting.

Output: Cleaned dataset saved in data/cleaned_crime_data.csv.

# Exploratory Data Analysis (EDA)

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

# Geographic Analysis

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

Total violent crimes by crime type (Urban vs Rural).html

Average violent crimes rate per 1000 (Urban vs rural).html

crime_timeline_animation.html

Notebooks: /notebooks/ directory

# Tools and Libraries

Python: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Folium, Prophet, GeoPandas.

Google Colab for Code Execution

GitHub for version control.

# Conclusion

This extensive examination of violent crimes in California between 2000 and 2013 indicates substantial temporal, regional, and categorical patterns in criminal behavior. Using cleansed crime data and spatial mappings by county and MPO region, we obtained many crucial insights:

Statewide Decline in Violent Crime: The total number of violent crime events is consistently decreasing across the state. This is corroborated both visually and by time-series forecasting with the Prophet model, which predicts further decline beyond 2013.

The Bay Area has routinely reported the greatest amount of violent crimes, owing to its vast population and urban congestion. However, its per capita crime rate remained reasonable, indicating a balance of population and crime volume.

Rural regions have higher per capita rates: Less populated areas, such as the Central/Southeast Sierra and Butte region, have higher average violent crime rates despite low total crime counts. This shows that individual risk exposure may be higher in some rural areas.

Crime Type Distribution Is Consistent: Aggravated assault is the most common violent crime in all geographic locations, followed by robbery and forced rape. Urban and rural locations have similar crime types, albeit numbers vary.

Geographical Variability Exists: County-level mapping revealed substantial contrasts. For example, Los Angeles County had the greatest crime rate and total count, while other rural counties had less activity. The interactive choropleth map effectively illustrates this discrepancy.

No Significant Correlation with region Codes Alone: The correlation matrix indicated that identifiers such as area codes or county FIPS alone do not strongly predict crime rates, highlighting the importance of temporal and categorical disaggregation, as performed in this study.

Overall, this research provides a multidimensional view of violent crime in California by integrating statistical modeling, interactive mapping, and region-specific analysis. These findings can help guide future resource allocation, public safety policies, and targeted intervention activities.

Author: Fahad Bin Hossain (2025).Project repository: [GitHub link here]
