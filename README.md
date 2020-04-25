# COVID-19-in-India

A dashboard to give an overview of the spread of the Novel Coronavirus COVID-19 pandemic across India, state-wise.

Link for the dashboard: https://srinathkr.shinyapps.io/COVID19-India/

## Summary (as of 13th April 2020, 12 pm)

![Summary](/Screenshots/Summary.png)

## Visualization (as of 13th April 2020, 12 pm)

![Visualization](/Screenshots/Visualization.png)

## Cumulative Trends (as of 13th April 2020, 12 pm)

![Cumulative Trends](/Screenshots/CumulativeTrends.png)

## Daily Trends (as of 13th April 2020, 12 pm)

![Daily Trends](/Screenshots/DailyTrends.png)

## About

**COVID-19 in India : A Dashboard** gives an overview of the spread of the Novel Coronavirus (COVID-19) pandemic across India, state-wise along with **SIR (Susceptible - Infectious - Recovered) model** for a period of 150 days starting from March 1. 

This dashboard has been made entirely using Rmarkdown framework.

**Data: **

[COVID-19 India API](https://api.covid19india.org/), a volunteer-driven API for COVID-19 stats & patient tracing in India.

**R packages used: **

* Dashboard - [flexdashboard](https://rmarkdown.rstudio.com/flexdashboard/) package.

* Table - [DT](https://rstudio.github.io/DT/) and [dplyr](https://dplyr.tidyverse.org/) packages.

* API Data - [rjson](https://www.rdocumentation.org/packages/rjson/versions/0.2.20) package.

* Modeling - [deSolve](http://desolve.r-forge.r-project.org/) and [lubridate](https://lubridate.tidyverse.org/) packages. 

* Visualizations - [plotly](https://plot.ly/r/), [ggplot2](https://ggplot2.tidyverse.org/), [geojsonio](https://ropensci.org/tutorials/geojsonio_tutorial/), [ggiraph](https://davidgohel.github.io/ggiraph/), [colormap](https://bhaskarvk.github.io/colormap/) and [hrbrthemes](https://hrbrmstr.github.io/hrbrthemes/) packages. 

**Note: **

For any other question or feedback, you can contact me on [LinkedIn](https://www.linkedin.com/in/srinath-kr-026147173/).

**Acknowledgement: **

Thanks for the API, [COVID-19 India API](https://api.covid19india.org/)!
