---
title       : Exploring mtcars
subtitle    : Create the regression model in one mouse click
author      : Pavel Burdanov
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation

All of you remember the Regression Models Course Project
where you tested different variable sets for the regression model...


```r
fit <- lm(mpg~cyl+hp+wt+am, data=mtcars)
summary(fit)
```

```
## 
## Call:
## lm(formula = mpg ~ cyl + hp + wt + am, data = mtcars)
## 
## Residuals:
##    Min     1Q Median     3Q    Max 
## -3.476 -1.847 -0.554  1.276  5.661 
## 
## Coefficients:
##             Estimate Std. Error t value Pr(>|t|)    
## (Intercept)  36.1465     3.1048   11.64  4.9e-12 ***
## cyl          -0.7452     0.5828   -1.28   0.2119    
## hp           -0.0250     0.0136   -1.83   0.0786 .  
## wt           -2.6065     0.9198   -2.83   0.0086 ** 
## am            1.4780     1.4411    1.03   0.3142    
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 2.51 on 27 degrees of freedom
## Multiple R-squared:  0.849,	Adjusted R-squared:  0.827 
## F-statistic:   38 on 4 and 27 DF,  p-value: 1.02e-10
```


I've found this process very tedious and have developed
the automated solution for this.

You can select the outcome and predictors and instantly run the model
without a line of R code.

Now you can add variables to your model in one mouse click!

---

## Solution

https://burdanovp.shinyapps.io/expmtcars

<iframe src="https://burdanovp.shinyapps.io/expmtcars"></iframe>

---

## Future Directions

- More output

- Ability to explore other datasets

- Variable interactions

- Model comparison with ANOVA

- Other types of regression models

- ???????

- PROFIT

--- .thank-you-slide

## Thank you!
