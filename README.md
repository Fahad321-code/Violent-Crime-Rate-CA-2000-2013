# Analysis of Violent Crime in California, 2000–2013

Summary

This study looks at the trends in violent crime in California counties and MPO areas between 2000 and 2013. The goal was to use Python-based data science algorithms to anticipate future crime trends and examine changes across time and regional patterns.

# Preprocessing of Data

Source: The California government's raw violent crime statistics (Data.gov).

# Steps for Cleaning:

Missing and inconsistent values were eliminated.

uniform column names.

Date formatting was changed and data types were confirmed.

Output: cleaned_crime_data.csv contains the cleaned dataset.

# Analysis of Exploratory Data (EDA)

# An overview of the statistics

descriptive statistics for population, count, and crime rate.

# Visuals:

Between 2000 and 2013, crime rates generally declined.

Box plots and scatter overlays are used to show the crime rate distribution by year.

Top Crime Types: Determined and categorized based on average frequency and number of crimes.

Correlations between numerical variables are displayed in a correlation matrix.

# Modeling Predictively (Prophet)

Prophet time series forecast is the model.

# Features of the input:

Report year: Observation year.

Rate: the quantity of violent crimes committed per 1,000 people.

# Results:

Crime rate projections through 2018.

Visualization of confidence intervals.

Conclusion: After 2013, predicted crime rates kept falling.

# Analysis of Geography

By MPO Region, Regional Trends:

A line graph showing the total number of crimes committed over time by MPO region.

Regional comparisons of average crime rates over time using both static and interactive graphics.

# Interactive visuals:

Choropleth Map: Geographical representation of county-level crime statistics.

Timeline with Animation: Annual Variations in Crime Rates by Area.

Crime Trends by Type (e.g., robbery, assault) in a Stacked Area Plot.

Comparing Urban and Rural Areas:

categorized counties based on region_name and geotype.

compared average crime rates with the total number of violent offenses.

While some rural counties had higher per capita rates, urban areas had more offenses overall.

# Results

cleaned_crime_data.csv is the cleaned dataset.

# HTML files that are interactive:

Violent crime geographic aalysis.html

Average violent crime rate over time (Top 5 MPO Regions)

Total Violent Crimes over time (Top 5 MPO Regions)

Distribution of crime types by MPO Region.html

Average violent crimes rate per 1000 (Urban vs rural)

Total Violent Crimes By Crime Type Urban and Rural.html

Heatmap of Total Violent Crimes by Crime Type and Year.html

# Libraries and Tools

Python: Seaborn, Plotly, Folium, Prophet, GeoPandas, NumPy, Matplotlib, and Pandas.

Google Colab for Executing Code 

For version control, use GitHub.

# conclusion

Significant temporal, regional, and categorical trends in criminal behavior are revealed by this thorough analysis of violent crimes in California from 2000 to 2013. We gained some important findings by using spatial mappings by county and MPO region and cleaned crime data:

Statewide Violent Crime Decline: Throughout the state, there has been a steady decline in the overall number of violent crime incidents. Both visual and time-series forecasting using the Prophet model, which projects additional decline after 2013, support this.

metropolitan Centers Lead in Total Crimes: Because of their dense populations and traffic, the Bay Area and other metropolitan areas recorded the highest rates of violent crimes. The population and crime volume were balanced, nevertheless, as evidenced by the reasonable per capita crime rates.

Rural Areas Have Greater Per Capita Rates: Although overall crime rates were low, violent crime rates were higher in less populous areas. This shows that in some rural locations, people may be more exposed to risk.

Consistent Distribution of Crime Types: In every region, aggravated assault was the most frequent violent crime, followed by robbery and forced rape.

Geographic Variability: Using interactive choropleth maps, county-level mapping demonstrated significant differences in crime rates and counts.

Region codes alone have little predictive value. Correlation analysis highlighted the need for comprehensive temporal and categorical analysis instead of depending only on region IDs.

Overall, by integrating statistical modeling, interactive mapping, and region-specific analysis, this study offers a multifaceted perspective on violent crime in California. Future resource allocation, public safety regulations, and focused intervention efforts can be guided by these findings.

Author: Fahad Bin Hossain (2025)

Project repository: https://github.com/Fahad321-code
