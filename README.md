# Apple-Watch-Health-Data
This repo will provide code for pulling Apple Watch Health data from Apple's Healthkit using the "AppleHealthAnalysis" rpackage by deepankardatta and converting the downloaded json file to a dataframe.

## Download "AppleHealthAnalysis" R Package
library(devtools)

intall_github("deepankardatta/AppleHealthAnalysis")

## How to Download Apple Health Data and Import to R
### 1) Open Apple Health and click the icon in the upper right corner
<img width="285" alt="screen shot 2018-02-24 at 1 23 00 pm" src="https://user-images.githubusercontent.com/36683142/36635299-3c1b624a-1967-11e8-9104-aa56fb871a11.png">

### 2) Export the Data
<img width="263" alt="screen shot 2018-02-24 at 1 24 04 pm" src="https://user-images.githubusercontent.com/36683142/36635295-1cd49fe6-1967-11e8-86cc-1c354b4933b5.png">

### 3) Email the Data
<img width="248" alt="screen shot 2018-02-24 at 1 26 30 pm" src="https://user-images.githubusercontent.com/36683142/36635261-c3c96c4c-1966-11e8-8366-c2b20ad3f795.png">
<img width="268" alt="screen shot 2018-02-24 at 1 27 36 pm" src="https://user-images.githubusercontent.com/36683142/36635268-d0a875b6-1966-11e8-8a7a-a4f02e9c89dc.png">

### 4) Open R
library(AppleHealthAnalysis)

health.data<- ah_import_xml("export.xml")

## Future Edits
I plan to edit this code to allow for interday summary of all variables as well as intraday variables within 10 minute bins.

## Resources
1. https://github.com/deepankardatta/AppleHealthAnalysis
2. https://gist.github.com/ryanpraski/ba9baee2583cfb1af88ca4ec62311a3d#file-apple_health_load_analysis_r-r
