# Preamble

In this intro we take you through a focused approach for using R to
generate data visualization elements from simulated data, this precise
focus aims to enable you to use R more comfortably for your data
visualization approaches. We will cover:

-   Installation
-   Set up
-   Data visualisation
-   Line plots
-   Area graph
-   Scatter plots
-   Animated graphs

# Installing R & RStudio

## Install R

R is the programming language you’ll be using. Go to:
<https://cran.r-project.org> Click on your operating system:

-   Windows → Click “Download R for Windows” → “base” → then click the
    .exe file to download.

-   macOS → Click “Download R for (Mac) OS X” → choose the .pkg file and
    install.

-   Linux → Follow instructions relevant to your Linux distribution.

## Install RStudio (Recommended IDE)

RStudio is a user-friendly interface for R. Note that R must be
installed before RStudio.

Go to: <https://posit.co/download/rstudio-desktop/>

-   Download the free version of RStudio Desktop for your OS.

-   Install it.

-   Run the installer and follow the default installation steps.

## Installing required packages

Open RStudio, you can run the following script to install the
recommended set of packages. These are widely used for data analysis and
report writing.

`install.packages(c("tidyverse", "ggplot2", "dplyr", "rmarkdown", "knitr"))`

## Posit Cloud

Alternatively you can use all of the codes we provide to you here on a
cloud version of R. For this:

-   Go to: <https://posit.cloud>

-   Click Sign Up (use your email, Google, GitHub, etc.)or Log In if you
    already have an account.

-   Once logged in, click “New Project”. This opens an RStudio
    environment in your browser — no installation needed.

# Set up

The following code chunk includes the required packages in this EDA.

    knitr::opts_chunk$set(echo = TRUE)

    if(!require(tidyverse)) install.packages("tidyverse", repos = "http://cran.us.r-project.org")
    if(!require(knitr)) install.packages("knitr", repos = "http://cran.us.r-project.org")
    if(!require(DT)) install.packages("knitr", repos = "http://cran.us.r-project.org")
    if(!require(plotly)) install.packages("plotly")
    if(!require(ggplot2)) install.packages("ggplot2")
    if(!require(dplyr)) install.packages("dplyr")
    if(!require(ggplot2)) install.packages("ggplot2")
    if(!require(gapminder)) install.packages("gapminder")
    if(!require(gganimate)) install.packages("gganimate")
    if(!require(ggalluvial)) install.packages("ggalluvial")

    # Load
    library(tidyverse)
    library(knitr)
    library(DT)
    library(plotly)
    library(ggplot2)
    library(dplyr)
    library(gapminder)
    library(ggalluvial)

# Data Visualisation

Creating data visualisation elements in R empowers you to explore,
communicate, and understand complex patterns in large scale data with
clarity and precision.

Through powerful packages like ggplot2, R enables the transformation of
raw numbers into meaningful, customisable visuals and reproducible data
visualistion elements. From simple line plots to interactive graphs and
dashboards.

This visual storytelling enhances transparency, supports
decision-making, and makes findings accessible to diverse audiences,
including those without technical backgrounds.

Please feel free to use the code provided to you in the Rmarkwon and run it in your local RStudio or Posit cloud to regenerate the graphs provided here. 
