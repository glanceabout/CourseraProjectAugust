---
title       : Data Products Project for Coursera
subtitle    : August 2015
author      : glanceabout
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : default       # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Overview

Our App provides managers and performance experts with the tools to 

> * guide evaluations of trainees or employees
> * examine various performance standards, and
> * explore potential recentering of rating guidelines

--- .class #id 

## Background

* Data-driven evaluations have become trainers and HR professionals' go-to option for assessing performance.

* However, often many 'subjective' evaluations are forced into too narrow an assessment rating by limited feedback options.

> * How much can be said about leadership by an integer between 1 and 5?

---

## The App

* The App loads evaluation data from .csv files when requested, and then freezes the averages onscreen as you propose various threshold standards

* This allows you to see how your personell are doing, in addition to whether it might be appropriate to adjust your standards

* See how the app rates the following average scores, as an example, against the threshold standard of 3:

* ***2.75 , 3.02, 3.95***


```
##            Item Average Evaluation Results
## 1    Leadership               2.75   -0.25
## 2 Communication               3.02    PASS
## 3  Organization               3.95    PASS
```


---

## Neat things I Learned

* For computing shinyUI elements on the fly, the library offers uiOutput() and renderUI() for dynamic ui items

> * I used this to populate a drop-down box with the list of students' data from which to choose

> * In the example app, the choices are hard-coded in a list. But my next step is to make them truly dynamically generated, just as the evaluation data are loaded from files when requested.




