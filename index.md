---

title       : Slidify application - BMI calculator
subtitle    : The presentation of the shiny application
author      : Ke Xiaobing
job         : System Engineer
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Introduction of the application

 * The Shiny app created for BMI calculator is displayed in the following screenshot.
 * Please be patient to wait around 10 seconds for page loading.
 * The app is user-friendly and easy to understand. The instructions of how to use this appliation can be found in the page.
 * You just need to manually enter your weight and height in left panel and click on "Submit" button. Then you could see calculation result in the right side.

---  

## App showcase
Try the application from here.

![screenshot](screen.png)

--- 

## BMI Calculation

The body mass index (BMI), or Quetelet index, is a measure of relative size based on the mass and height of an individual.

The index was devised by Adolphe Quetelet during the course of developing what he called "social physics", between 1830 and 1850. The BMI for a person is defined as their body mass divided by the square of their height-with the value universally being given in units of kg/m2. If an individual has weight 60kg and height 1.65 meter, the BMI calculation is as follows.


```r
weight <- 60.00
height <- 1.65
BMI <- round((weight / (height * height)), digits = 1)
BMI
```

```
## [1] 22
```

--- 

## BMI Category
A frequent use of the BMI is to assess how much an individual's body weight departs from what is normal or desirable for a person of his or her height. The weight excess or deficiency may, in part, be accounted for by body fat (adipose tissue) although other factors such as muscularity also affect BMI significantly. The WHO regards a BMI of less than 18.5 as underweight and may indicate malnutrition, an eating disorder, or other health problems, while a BMI greater than 25 is considered overweight. These ranges of BMI values are valid only as statistical categories.

* BMI < 18.5: Underweight
* 18.5 < BMI < 25: Normal
* BMI > 25: Overweight
