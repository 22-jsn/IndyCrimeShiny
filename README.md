
##  IndyCrimeShiny

**Project Overview**

This Shiny application analyzes the relationship between unemployment rates and different types of crimes in Indiana for the year 2023. The purpose of this research is to uncover patterns or correlations that might exist between economic conditions and criminal behavior.

**Why This Topic?**

Crime and unemployment are often interconnected. By exploring real data from Indiana, we wanted to investigate whether rising unemployment aligns with increased incidents of certain crimes or crimes in general.

**Project Requirements**

Used Shiny app with multiple visualization tabs

Integrated two related datasets: 2023 Indiana crime records from Kaggle and 2023 Indiana unemployment data from fred.stlouis.org

Detailed documentation of project scope and steps taken

Included dropdown filters for month and offense type

Displayed backlog of visualizations and analysis ideas


**Scope of Project**

The scope involved merging state-level monthly crime data with unemployment statistics, creating meaningful visualizations, and exploring insights from correlations between crime types and unemployment. Filtering was 
done by offense, county, age group, race, and gender.


**Backlog & Future Concepts**

Predictive Modeling: Future versions of this project could incorporate statistical or machine learning models (e.g., linear regression, random forest) to predict crime rates based on unemployment trends, demographic shifts, or regional differences. This would allow the dashboard to move beyond observation and into forecasting.

Policy Impact Analysis: Investigating the effect of state programs—such as workforce development, mental health support, or post-incarceration services—on crime rates could offer practical policy insights. This would require merging program implementation timelines with crime data.

Multi-State Comparison: Expanding the project to include crime and unemployment data from neighboring states like Illinois, Ohio, or Michigan could place Indiana’s trends in context. Comparative analysis would help 
determine whether observed patterns are consistent regionally or state-specific.

Geospatial Mapping: Adding geospatial visualizations using tools like leaflet or sf could help identify crime hot spots across Indiana. Mapping crimes by county or ZIP code would enhance spatial analysis and offer location-based insights for local policy and law enforcement.

Time-Lagged Unemployment Effects: A more advanced approach could analyze the lag between rising unemployment and subsequent crime increases. This time-series strategy would allow exploration of delayed effects and could support stronger causal inferences.

**Libraries & Technologies Used**

- **R** – Statistical computing and visualization
- **Shiny** – Building interactive web applications
- **ggplot2** – Data visualization
- **plotly** – Interactive charts and graphs
- **dplyr** – Data manipulation and cleaning
- **readr** – Reading and writing data files
- **tidyr** – Data reshaping and tidying
- **DT** – Rendering interactive data tables within Shiny

All development and visualization were done using **RStudio**.
