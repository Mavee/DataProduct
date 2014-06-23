---
title       : Diamond Price Prediction
subtitle    : Shiny Application
author      : M.K.
job         : Aspiring DataScientist  
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
github:
 user: Mavee
 repo: DataProduct
---

### Overview

"Diamonds are Forever" - so why not buy one for your loved one?  You can use this cool app to estimate the price of diamond rings.

The Diamond Price Prediction is a shiny application that calculates the predicted price (in USD) for diamonds when the diamond weights (in carats) are input by users.

### Description of the Application

The 'Diamond Price Predication' application has a simple interface wherein you enter the weight of the diamond (in carats) on the left sidebar panel and click the 'submit' button.  The price of the diamond is then displayed on the righthand side main panel.  The price is shown is U.S. Dollars.  Since the original dataset(diamond) has prices in Singapore dollars, the application converts the price in Singapore $ to USD using the average exchange rate of 1 Singapore $=0.80 USD.  

The application also displays the mean values for data in the diamond dataset.  To see the mean value for the price of diamond, converted from Singapore$ to USD, select the checkbox for the mean diamond price and click 'submit'. Similarly to see the mean value of the diamond weights in the diamond dataset, select the checkbox for the mean diamond weight and click 'submit'. The application always displays predicted diamond price for 0.1 carat diamond on startup.

--- .class #1

## Dataset for Prediction Model 

The shiny application 'Diamond Price Prediction' is based on the R devtools dataset 'diamond'.   This is a data set on 48 diamond rings containing price in Singapore dollars and the size of the diamond in carats.  

Shown below are the top 6 rows of data in the diamond dataset.



```r
head(diamond)
```

```
##   carat price
## 1  0.17   355
## 2  0.16   328
## 3  0.17   350
## 4  0.18   325
## 5  0.25   642
## 6  0.16   342
```


--- .class #2

## Application User Interface Screen

Here is the main screen for 'Diamond Data Prediction' application on startup.

![image](assets/img/DiamondAppScr1.jpg)


--- .class #3

## Application Screen Showing Results

Here is the application screen with output predicting the price for 0.3 carat diamond and showing the mean values for carat and price from the diamond dataset.

![image](assets/img/DiamondAppScr2.jpg)

Caution!  Diamonds Are Forever BUT Diamond Prices Are Not Forever!


