---
title: "Map Project"
author: "Kinara Gajjar"
date: "14/08/2020"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## June 15, 2020

```{r}
library(leaflet)
CollegeIcon <- makeIcon(
  iconUrl =  "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQtHTGOR0lAT4urPGcmLQ3EmIqqicHbCQV2SQ&usqp=CAU",
  iconWidth = 50, iconHeight = 50,
  iconAnchorX = 50, iconAnchorY = 50
)

my_map <- leaflet() %>%
  addTiles()%>%
  addMarkers(lat=24.576110,lng=73.700500,icon = CollegeIcon)
```

## June 15, 2020

```{r, echo=FALSE}
my_map
```
