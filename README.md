# COVID-19 in India : An Analysis

A shiny R dashboard to give an overview of the spread of the Novel Coronavirus COVID-19 pandemic across India, state-wise along with **SIR (Susceptible - Infectious - Recovered) model** for a period of 150 days starting from March 2. 

Link for the dashboard: https://srinathkr.shinyapps.io/COVID19-India/

(The site takes some time to load, so please bear with it!)

## Summary (as of 9th May 2020, 12:30 pm)

![Summary](/Screenshots/Summary.png)

## Visualization (as of 9th May 2020, 12:30 pm)

![Visualization](/Screenshots/Visualization.png)

## Cumulative Trends (as of 9th May 2020, 12:30 pm)

![Cumulative Trends](/Screenshots/CumulativeTrends.png)

## Daily Trends (as of 9th May 2020, 12:30 pm)

![Daily Trends](/Screenshots/DailyTrends.png)

## SIR Model

### Introduction

Compartmental models simplify the mathematical modelling of infectious diseases. The **SIR model** is one of the simplest compartmental models, and many models are derivatives of this basic form. 

The model consists of three compartments: 

- **S** for the number of **susceptible**, 
- **I** for the number of **infectious**, and 
- **R** for the number of **recovered** or deceased individuals. 

This model is reasonably predictive for infectious diseases that are transmitted from human to human. 

### Predicted vs Observed cases (as of 9th May 2020)

![Predicted vs Observed cases](/Screenshots/SIRModel1.png)

### Predicted vs Observed cases (Log-linear) (as of 9th May 2020)

![Predicted vs Observed cases (Log-linear)](/Screenshots/SIRModel2.png)

### Math in the model

#### Equations

The SIR system without so-called vital dynamics (birth and death, sometimes called demography) can be expressed by the following set of ordinary differential equations (ODEs): 

![Equation 1](https://wikimedia.org/api/rest_v1/media/math/render/svg/29728a7d4bebe8197dca7d873d81b9dce954522e)

where **S** is the stock of susceptible population, **I** is the stock of infected, **R** is the stock of removed population (either by death or recovery), and **N** is the sum of these three.

Note that from:

![Equation 2](https://wikimedia.org/api/rest_v1/media/math/render/svg/8edc1234df2c16e511f3c417cfd1720c1086de05)

it follows that:

![Equation 3](https://wikimedia.org/api/rest_v1/media/math/render/svg/4ef2c489d7916e880a3bccc6f85ccae3fb2f79a3)

expressing in mathematical terms the constancy of population N.

#### R0

The dynamics of the infectious class depends on the following ratio:

![Equation 4](https://wikimedia.org/api/rest_v1/media/math/render/svg/4aae42f8253a395c52a798a9ad5a7e4adb6fceea)

the so-called **Basic Reproduction number** (also called basic reproduction ratio). **R0** (pronounced “R-naught”) is the rate at which a virus is transmitted. It indicates the **average number of people who will contract the virus from a person who has already been infected**, in a population where all subjects are susceptible. 

### Prediction of infectious cases (as of 9th May 2020)

![Prediction of infectious cases](/Screenshots/SIRModel3.png)

### Prediction of infectious cases (Log-linear) (as of 9th May 2020)

![Prediction of infectious cases (Log-linear)](/Screenshots/SIRModel4.png)

### Note

This is a **worst case prediction** and should be taken with a lot of caution. Not surprisingly, it can be wrong. On one hand, this is based on rather unrealistic assumptions (for example, no public health interventions, fixed Reproduction number, etc.). On the other hand, we still have to be careful and strictly follow public health interventions because previous pandemics such as H1N1 and Spanish flu have shown that incredibly high numbers are not impossible! 

## About

This dashboard/tracker gives an overview of the spread of the Novel Coronavirus (COVID-19) pandemic across India, state-wise along with **SIR (Susceptible - Infectious - Recovered) model** for a period of 150 days starting from March 2. 

This application has been made entirely using Rmarkdown framework.

**R packages used:**

* Dashboard - [flexdashboard](https://rmarkdown.rstudio.com/flexdashboard/) package.

* Table - [DT](https://rstudio.github.io/DT/) and [dplyr](https://dplyr.tidyverse.org/) packages.

* API Data - [rjson](https://www.rdocumentation.org/packages/rjson/versions/0.2.20) package.

* Modeling - [deSolve](http://desolve.r-forge.r-project.org/) and [lubridate](https://lubridate.tidyverse.org/) packages. 

* Visualizations - [plotly](https://plot.ly/r/), [ggplot2](https://ggplot2.tidyverse.org/), [geojsonio](https://ropensci.org/tutorials/geojsonio_tutorial/), [ggiraph](https://davidgohel.github.io/ggiraph/), [colormap](https://bhaskarvk.github.io/colormap/) and [hrbrthemes](https://hrbrmstr.github.io/hrbrthemes/) packages. 

## FAQ

**Are you official?**

No.

**Who are you?**

I am an enthusiastic developer and a data analyst who wanted to do contribute to India's fight against COVID-19.

**Is the project open sourced?**

Yes! The project is completely open sourced. You can find the link to the GitHub repo [here](https://github.com/srinathkr07/COVID-19-in-India/).

**From where do you get the data?**

Data collected by a group of volunteers is validated and published into a Google sheet and an API. Thanks for the API, [COVID-19 India API](https://api.covid19india.org/)! 

**Is the SIR model accurate?**

I am not a specialist in Epidemiology so there are bound to be differences between actual and predicted cases. These predictions are only meant to be taken as a worst case scenario and with a lot of caution. 
