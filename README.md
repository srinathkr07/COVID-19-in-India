# COVID-19-in-India

https://srinathkr.shinyapps.io/COVID19-India/

![Screenshot](/Screenshots/COVID19.png)

This simple dashboard gives an overview of the spread of the Novel Coronavirus COVID-19 pandemic across India, state-wise. 
This dashboard has been made entirely using Rmarkdown framework.

**Data source**

[Ministry of Health and Family Welfare, India](https://www.mohfw.gov.in/).

**R packages used**

* Dashboard - [flexdashboard](https://rmarkdown.rstudio.com/flexdashboard/) package.

* Table - [dplyr](https://dplyr.tidyverse.org/), [tidyr](https://tidyr.tidyverse.org/) and [DT](https://rstudio.github.io/DT/) packages.

* Scraping - [rvest](http://rvest.tidyverse.org/), [magrittr](https://cran.r-project.org/web/packages/magrittr/vignettes/magrittr.html), [xml2](https://xml2.r-lib.org/) and [stringr](https://stringr.tidyverse.org/) packages.

* Map Visualization - [ggplot2](https://ggplot2.tidyverse.org/), [geojsonio](https://ropensci.org/tutorials/geojsonio_tutorial/), [ggiraph](https://davidgohel.github.io/ggiraph/), [colormap](https://bhaskarvk.github.io/colormap/) and [hrbrthemes](https://hrbrmstr.github.io/hrbrthemes/) packages. 

**Note**

Since the data is scraped from [Ministry of Health and Family Welfare, India](https://www.mohfw.gov.in/) and **the format of the page is changed often**, one might not be able to see the stats and visualisation, if the page format doesn't match with the one I have coded for. 
