---
title       : Prediction using MTCars Data
subtitle    : 
author      : Sumukh
job         : Creator of awesome apps :P
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Need for the App

1. MTCars is one of the most popular datasets out there
2. Used to teach linear regression to staudents of statistics
3. It is quite simple: it has just 32 observations
4. But it has 11 variables !!

--- .class #id 

## Features
1. You can create scatterplot between any two variables
2. I have selected 4 continous variables
3. It shows a regression line as well
4. You can give a value of x-variable for which you want to predict y-value
5. It will use this for predicting the Y-variable value based on the regression line

--- .class #id

## Instructions
1. Select the radio buttons to select the X and Y variables
2. Optionally enter the X-variable's value in the text box if you want to
3. Press submit
4. Blink your eyes
5. The answers are on the screen !!

--- .class #id

## How to predict Y-values

1. use lm(mtcars$y~mtcars$x)
2. This will give you a regression object
3. The object has a coefficients attribute
4. This will give you alpha and beta values

(Calculations done by Slidify)

```r
# What you entered
x <- 9.4

# Alpha and Beta values in regression equation
y<-1.3+4.8*x

#Predicted value of Y
y
```

```
## [1] 46.42
```

--- .class #id

## Benefits of using the App
1. Good for cross-checking calculations
2. Understand relations between the variables
   For example, Mileage(miles/gallon of fuel) decreases with increase in weight
   which implies negative correlation
3. You can cross-check your calculations using the prediction scores
