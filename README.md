Trends in I-O Psychology
================

## Trends in Industrial-Organizational Psychology

As scientists look for new empirical insights in the world of industrial-organizational
(I–O) psychology, topics inevitably fall in and out of vogue.  Perhaps the most volatile
and well recognized shifts have been observed among the personality research domain.
Namely, Walter Mischel’s 1968 book *Personality and Assessment* gloomy concluded: "\[w\]ith
the possible exception of intelligence, highly generalized behavioral consistencies have
not been demonstrated, and the concept of personality traits as broad response
predispositions is thus untenable."  After this book was published, personality research
considerably declined for the following decade.  Identifying such research trends (and slumps)
helps researchers and practitioners determine where the field has been and is headed in
addition to identify ideas and topics that warrant empirical investigations and/or should be
reexamined.

This Shiny app was designed to help researchers and practitioners identify current trends in
I–O psychology.  It uses user-specified queries to search peer-reviewed article abstracts in I-O
psychology's top scientific journals (see Aguinis et al., 2017).  Search results are plotted over
time, and users are able to narrow down specific journals and download a .csv file of their
generated data.  Additionally, search results are used to predict citation rates across decades.
Feel free to download and adapt the app to your needs or submit a request.

## System Requirements

In addition to R and RStudio, this app requires the following packages:

1. shiny
2. shinyBS
3. shinydashboard
4. tidyverse
5. tidytext
6. plotly
7. knitr
8. vroom

Dependencies can be easily installed and loaded via the following `R` code.

``` r
source("https://raw.githubusercontent.com/zktraylor/trends_in_io/master/install_dependencies.R")
```

## Run the Shiny App

Clone/download the repository using git (e.g., download as .zip) and run the following code in your RStudio console.

``` r
# cloned/downloaded file is named `~/shiny_example`
# set as working directory
setwd("~/shiny_example")
```

## Screenshots

![Overview](supl/dashboard.PNG)

![Results](supl/search_results.png)

![Trend by Publication Outlet](supl/journal_selection.png)

## Change Logs

### September 2026

- Migrated Shiny app to [zktraylor](https://www.github.com/zktraylor/trends_in_io)

## Old Change Logs

### January 2020

- Significant speed improvements
- Internal reorganization
- Action button for new search

### October 2019

- Added ability to quickly select and deselect all journals
- Completely overhauled UI
- Refined outputted visualizations

### September 2019

- Expanded database coverage to include 30 additional journals
- Included citation-rate visualization
- Implemented data import via `vroom` to increase speed
- UI update
- Aesthetic improvements
- Code improvements and clarity
