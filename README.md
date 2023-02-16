# Getting_cleaning_data

title: "Data-cleaning"
author: "Mario Gomez"
date: "2023-02-16"
output:
  pdf_document: default
  html_document: default
---


### Downloading Files

Here we show how we download files from the web

```{r}
#create an object with the URL
fileURL <- "https://data.baltimorecity.gov/api/views/dz54-2aru/rows.csv?accessType=DOWNLOAD"
#then use the download.file function  with a detinity library and  the method curl since this is a http (secure?)
download.file(fileURL, destfile = "~/Coursera/Data_science_specialization/Getting_cleaning_data/cameras.csv", method = "curl")
list.files("~/Coursera/Data_science_specialization/Getting_cleaning_data/")
```

```{r}
#we can also keep the date the data was downloaded
dateDownloaded <- date()
dateDownloaded
```
```{r}
data("iris")
plot(iris$Species,iris$Petal.Length)
```
```{r}
#extra information...
library(ggplot2)
```
