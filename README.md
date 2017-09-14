# R course

## Introduction to handling big data with dplyr and data.table.

For the course we will first need to download the following data which consists of 2 sets of files, `Coupon` and `Ticket`.
They can be both downloaded at https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=289 and https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=272 respectively.

When downloading the files, as selecting all variables will result on two large files, please select the variables on the table below. Note that Coupon and Ticket have different variables.

```R
Coupon = "Itinerary ID", "Market ID", "Sequence Number", "Origin City Market ID",  
"Origin", "Year", "Quarter", "Destination City Market ID", "Destination", "Trip Break", "Operating Carrier", 
"Distance", "Gateway"

Ticket = "Itinerary ID", "Roundtrip", "Itinerary Yield", "Passengers",
"Itinerary Fare", "Bulkfare Indicator", "Distance Full"
```

We assume that RStudio has been properly installed, with the latest R version available.

After downloading the files, please install the Data.Table and Dplyr packages by typing the code mentioned below on your RStudio console.

```R
install.packages("data.table")
install.packages("dplyr")
```
