This package constitutes an interactive R problem set based on the RTutor package (https://github.com/skranz/RTutor). 

---
This problem set guides the user throug the paper "Wall Street and the Housing Bubble" by Ing-Haw Cheng, Sahil Raina and Wei Xiong, which can be found here: [link](https://www.aeaweb.org/articles?id=10.1257/aer.104.9.2797)
---

## 1. Installation

RTutor and this package is hosted on Github. To install everything, run the following code in your R console.
```s
if (!require(devtools))
  install.packages("devtools")
source_gist("gist.github.com/skranz/fad6062e5462c9d0efe4")
install.rtutor(update.github=TRUE)

devtools::install_github("mwentz93/RTutorWallStreet", upgrade_dependencies=FALSE)
```

## 2. Show and work on the problem set
To start the problem set first create a working directory in which files like the data sets and your solution will be stored. Then adapt and run the following code.
```s
library(RTutorWallStreet)

# Adapt your working directory to an existing folder
setwd("C:/problemsets/RTutorWallStreet")
# Adapt your user name
run.ps(user.name="Jon Doe", package="RTutorWallStreet",
       load.sav=TRUE, sample.solution=FALSE)
```
If everything works fine, a browser window should open, in which you can start exploring the problem set.
