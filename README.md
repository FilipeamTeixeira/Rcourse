# R course

## Introduction to handling big data with dplyr and data.table.

For the course we will first need to download the following data which consists of 2 sets of files, `Coupon` and `Ticket`.
They can be both downloaded at https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=289 and https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=272 respectively.

Lets start by selecting for both files the 1st Quarter of 2011.
When downloading the files, as selecting all variables will result on two large files, please select the variables on the table below. Note that Coupon and Ticket have different variables.

```R
Coupon = "Itinerary ID", "Market ID", "Sequence Number", "Origin City Market ID",  
"Origin", "Year", "Quarter", "Destination City Market ID", "Destination", "Trip Break", "Operating Carrier", 
"Distance", "Gateway"

Ticket = "Itinerary ID", "Roundtrip", "Itinerary Yield", "Passengers",
"Itinerary Fare", "Bulkfare Indicator", "Distance Full"
```

We assume that RStudio has been properly installed, with the latest R version available.


### Preparing the project

Start a new project, and copy the .R files included with this repository to its root folder.
Don't forget to copy as well as the downloaded csv files into a folder named data.
Rename the files to `Coupon 2011Q1.csv` and `Ticket 2011Q1.csv` respectively. Usually it is possible to go around renaming the files but I'll leave that for another course.

After, please install the Data.Table and Dplyr packages by typing the code mentioned below on your RStudio console.

```R
install.packages("data.table")
install.packages("dplyr")
```
