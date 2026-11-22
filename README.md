This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

The problem set is based on the paper **"Taxing Billionaires: Estate Taxes and the Geographical Location of the Ultra-Wealthy"** by Enrico Moretti and Daniel J. Wilson (2023).

Link to the paper: https://doi.org/10.1257/pol.20200685

In this problem set, we examine whether state-level estate taxes influence where the wealthiest Americans choose to live. Using data on the Forbes 400, we look at how the geographic distribution of billionaires has developed over time and estimate how strongly they respond to estate taxes. Building on these results, we evaluate whether introducing an estate tax pays off for a state, taking into account both the additional tax revenue and the losses from billionaires moving away.

You can also explore the interactive problem set directly in your browser without installing the R package. Please note that your progress cannot be saved in the online version.

Online version: https://tassilogeiselhart.shinyapps.io/ErbschaftsteuerUSA/

To install and work through the problem set locally, follow the steps below.

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
install.packages("RTutor",repos = c("https://skranz-repo.github.io/drat/",getOption("repos")))

if (!require(devtools))
  install.packages("devtools")

devtools::install_github("tassilogeiselhart/RTutorErbschaftsteuerUSA")
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorErbschaftsteuerUSA)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorErbschaftsteuerUSA")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorErbschaftsteuerUSA",
       auto.save.code=TRUE, clear.user=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
