# Apple-Watch-Health-Data
This repo will provide code for pulling Apple Watch Health data from Apple's Healthkit using the "AppleHealthAnalysis" rpackage by deepankardatta and converting the downloaded json file to a dataframe.

## Download "AppleHealthAnalysis" R Package
library(devtools)
intall_github("deepankardatta/AppleHealthAnalysis")
library(AppleHealthAnalysis)

## How to Download Apple Health Data and Import to R
### 1) Open Apple Health and click the icon in the upper right corner
<img width="255" alt="screen shot 2018-02-24 at 1 11 16 pm" src="https://user-images.githubusercontent.com/36683142/36635102-3fe1cdf4-1964-11e8-851d-8e758d1f6eb0.png">

### 2) Export your Apple Health Data
<img width="283" alt="screen shot 2018-02-24 at 1 09 53 pm" src="https://user-images.githubusercontent.com/36683142/36635115-5e7cbc10-1964-11e8-9ad5-de5b5317303d.png">

### 3) Open R
health.data<- ah_import_xml("export.xml")

## Future Edits
I plan to edit this code to allow for interday summary of all variables as well as intraday variables within 10 minute bins.

## Resources
1. https://github.com/deepankardatta/AppleHealthAnalysis
2. https://gist.github.com/ryanpraski/ba9baee2583cfb1af88ca4ec62311a3d#file-apple_health_load_analysis_r-r
