
##  IndyCrimeShiny

**Project Overview**

This Shiny application analyzes the relationship between unemployment rates and different types of crimes in Indiana for the year 2023. The purpose of this research is to uncover patterns or correlations that might exist between economic conditions and criminal behavior.

**Why This Topic?**

Crime and unemployment are often interconnected. By exploring real data from Indiana, we wanted to investigate whether rising unemployment aligns with increased incidents of certain crimes or crimes in general.

**Project Requirements**

Used Shiny app with multiple visualization tabs
 tabPanel("Top Crimes by Month", plotlyOutput("topCrimeMonth")),
    tabPanel("Crime by Gender", plotlyOutput("genderCrimePlot")),

Integrated two related datasets: 2023 Indiana crime records from Kaggle and 2023 Indiana unemployment data from fred.stlouis.org
crime_data <- read.csv("final_grouped_clean_indiana_crime_unemployment_2023.csv")

Detailed documentation of project scope and steps taken

Included dropdown filters for month and offense type

Displayed backlog of visualizations and analysis ideas
h4("Backlog & Future Concepts"),
      tags$ul(
        tags$li("Predictive Modeling: Future versions of this project could incorporate statistical or machine learning models (e.g., linear regression, random forest) to predict crime rates based on unemployment trends, demographic shifts, or regional differences. This would allow the dashboard to move beyond observation and into forecasting."),


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

library(shiny)
library(ggplot2)
library(dplyr)
library(plotly)
library(DT)

- **R** – Statistical computing and visualization
- **Shiny** – Building interactive web applications
- **ggplot2** – Data visualization
- **plotly** – Interactive charts and graphs
- **dplyr** – Data manipulation and cleaning
- **readr** – Reading and writing data files
- **tidyr** – Data reshaping and tidying
- **DT** – Rendering interactive data tables within Shiny

## GitHub Project Management

This project was managed using a Kanban board on GitHub Projects. As the sole team member, I created and tracked all key stages of work — from planning and dataset cleaning to visualization building and final documentation. The board is organized into five columns:

- **Backlog**: Idea generation, early planning and future improvements
- **Ready**: Data merging, cleaning, and UI planning
- **In Progress**: Chart creation, filtering logic, and design
- **In Review**: Debugging and final labeling improvements
- **Done**: Completed milestones including dataset uploads and documentation


**Prediction Model Rationale**

Model I Chose: Linear Regression

I selected linear regression because it is widely used for analyzing relationships between continuous variables. My primary research question involves whether changes in unemployment rates correlate with changes in crime counts, which is well suited for a regression framework. Linear regression provides interpretability, ease of implementation, and is commonly used in economic and social science research.

LLM-Suggested Model: Random Forest

I asked ChatGPT to recommend a predictive model suitable for my dataset. It suggested using a Random Forest Regressor, citing its robustness to overfitting, ability to handle nonlinear relationships, and effectiveness on mixed-type datasets. The model was recommended based on its frequent use in criminology and social science forecasting tasks.
Supporting Research Article

ChatGPT identified the following peer-reviewed paper:

Title: A Random Forest Approach to Forecasting Urban Crime Rates
Authors: Zhang, X., & Zhao, J. (2020)
Journal: Crime Science, Vol. 9, Article 5
Summary: The authors used Random Forest models to forecast crime across multiple U.S. cities using socioeconomic indicators such as unemployment, poverty rate, and educational attainment. Their results showed that RF models outperformed linear models in terms of accuracy and flexibility, especially when predicting violent crimes and property thefts.
Zhang, X., & Zhao, J. (2020). A random forest approach to forecasting urban crime rates. Crime Science, 9(5). https://doi.org/10.1186/s40163-020-00124-3

This study applied a Random Forest model to predict crime in urban areas using socioeconomic predictors such as unemployment, education, and income levels. The model outperformed traditional linear models in both accuracy and generalizability, especially when predicting violent and property crimes. The non-parametric nature of Random Forest allowed it to capture complex, non-linear dynamics present in urban crime data.

Relevance to My Project

My dataset shares structural similarities with the research cited, incorporating monthly unemployment rates and detailed crime breakdowns by type, gender, age, and race. Given the strong predictive performance observed in the Zhang and Zhao (2020) study, Random Forest would be a fitting model for future expansion of this project beyond visualization. It would allow for robust forecasting and potentially inform local policy decisions through scenario modeling.

