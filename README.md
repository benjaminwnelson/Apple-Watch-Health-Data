# Apple-Watch-Health-Data
This repo will provide code for pulling Apple Watch Health data from Apple's Healthkit using the "AppleHealthAnalysis" rpackage by deepankardatta and converting the downloaded json file to a dataframe.

##Download "AppleHealthAnalysis" R Package
library(devtools)
intall_github("deepankardatta/AppleHealthAnalysis")
library(AppleHealthAnalysis)

##Download Apple Health Data
-First open Apple Health and click the icon in the upper right corner

