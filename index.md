---
framework   : impressjs   # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
github: {user: patilv, repo: slidifyandimpressjs}
mode        : selfcontained # {standalone, draft}


---  x:0 y:0 z:0 rotx:-40 roty:-10 

<br><br><br><br><br><br><br>

## Using Impress.js Framework for Presentations
  
Created using Slidify <br><br>
<super> Vivek Patil 

---  x:-6000 y:2000 z:90 rotx:180 roty:-360 
  
## Task at hand
  
1. Impress.js provided an **impressive** framework but creating boring presentations for classes was difficult using the style sheet. 
2. So, attempted to create a custom one for some basic functionality by taking elements from the impress.js demo css, io2012 sample css, and some html tags.
3. This code can be improved upon in a significant manner.

---  x:-2000 y:0 z:0 rotx:-90 roty:-90 
  
## Ordered list
  
This list should be ordered
<ol>
1. Point 1<br>
2. Point 2<br>
3. Point 3

---  x:-2000 y:2000 z:1000 rotx:-75 roty:-75 
  
## Unordered with bullet points
  
This list should be unordered with bullet points

1. Point 1
2. Point 2
3. Point 3

---  x:-2000 y:-2000 z:-1000 rotx:45 roty:90 

## Unordered with neither bullets nor numbers
  
This list should be unordered with neither bullets nor numbers

Point 1 <br>
Point 2 <br>
Point 3

---  x:0 y:-4000 z:-2000 rotx:-40 roty:-10 

## Two column slide

This is a slide with a two column layout.

Column X | Column Y 
---------|----------
Row 1 of Column 1    | Row 1 of Column 2    
Row 2 of Column 1    | Row 2 of Column 2    

---  x:2000 y:-2000 z:500 rotx:-75 roty:75   

## Two column slide with only one row?

Whether borders are visible are not can be controlled using the css sheet

Column X | Column Y 
---------|----------


---  x:2000 y:2000 z:-1000 rotx:120 roty:-120 
  
## Three Columns here
  
Three column table here, with one entry being a link to the R-Project

Column X | Column Y | Column Z
---------|----------|---------
Row 1    | Row 1    |  Row 1
Row 2    | Row 2    |  <a href="http://www.r-project.org" target="_blank"><img src="http://www.r-project.org/Rlogo.jpg" alt="R" title="R"width= "35" height = "35" ></a>


---  x:2000 y:0 z:1000 rotx:70 roty:90

## Some R code and output

Head of iris


```r
head(iris)
```

```
##   Sepal.Length Sepal.Width Petal.Length Petal.Width Species
## 1          5.1         3.5          1.4         0.2  setosa
## 2          4.9         3.0          1.4         0.2  setosa
## 3          4.7         3.2          1.3         0.2  setosa
## 4          4.6         3.1          1.5         0.2  setosa
## 5          5.0         3.6          1.4         0.2  setosa
## 6          5.4         3.9          1.7         0.4  setosa
```

Tail of iris


```r
tail(iris)
```

```
##     Sepal.Length Sepal.Width Petal.Length Petal.Width   Species
## 145          6.7         3.3          5.7         2.5 virginica
## 146          6.7         3.0          5.2         2.3 virginica
## 147          6.3         2.5          5.0         1.9 virginica
## 148          6.5         3.0          5.2         2.0 virginica
## 149          6.2         3.4          5.4         2.3 virginica
## 150          5.9         3.0          5.1         1.8 virginica
```


--- x:0 y:2000 z:2000 rotx:100 roty:-100 

## Code and a plot


```r
library(ggplot2)
ggplot(iris, aes(x = Sepal.Length, y = Petal.Length, color = Species)) + geom_point() + 
    geom_smooth(method = loess)
```

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3.png) 


---   x:0 y:4000 z:-2000 rotx:-190 roty:190 

## Embedding another page 

<iframe src="http://www.rstudio.com/" style="min-height: 500px; min-width: 750px;"></iframe>

--- x:2000 y:4000 z:1500 rotx:190 roty:-190

## Embedding a Video

Let's watch the newly created video about R from Revolution Analytics  
<center>
<iframe width="640" height="360" src="http://www.youtube.com/embed/TR2bHSJ_eck?feature=player_embedded" frameborder="0" allowfullscreen></iframe>

---- x:4000 y:4000 z:2500 rotx:-180 roty:360

## Acknowledgements

1. Bartek Szopka for <a href="https://github.com/bartaz/impress.js" target="_blank"> Impress.js </a>
2. Eric Bidelman and Luke Mahe for <a href="https://code.google.com/p/io-2012-slides/" target="_blank">Google IO 2012</a>
3. Ramnath Vaidyanathan for adapting the above frameworks for <a href="http://slidify.org/" target="_blank"> Slidify </a> and for his prompt responses to queries 
4. The generous R-community 





