---
title       : Slidify Template 
subtitle    : Using Lehigh colors
author      : Alex Pacheco
job         : LTS Research Computing
logo        : lu.png
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
license     : by-sa
---  .lehigh

## Read-And-Delete

1. Edit YAML front matter
2. Write using R Markdown
3. Use an empty line followed by three dashes to separate slides!
   * To use my template using Lehigh's  colors use "---  .lehigh" instead. 

--- .lehigh

## My modification to the css formatting

1. To use two columns , use add "&twocol_width to the slide separator"
2. Each column should be preceeded with "*** =alignment width:x%"
    * For e.g. "*** =left width:30%" and "*** =right width:70%" will create two columns with 30:70 ration between left and right columns

--- .lehigh

## Creating presentations using Slidify

* Install the `devtools` package and load it


```r
install.packages('devtools')
library(devtools)
```

* Install the `slidify` and `slidifyLibraries` package from github


```r
install_github('ramnathv/slidify')
install_github('ramnathv/slidifyLibraries')
```

* if you get an error, try 


```r
install_git('https://github.com/ramnathv/slidify.git') 
install_git('https://github.com/ramnathv/slidifyLibraries.git')
```

* Load the slidify library


```r
library(slidify)
```

--- .lehigh

## Creating presentations using Slidify (contd)

* Create a Slide desk

```r
author("myslides")
```

* This will create a folder called `myslides` with files and subdirectories to create your presentation
   - `assets/css/custom.css`: Create your own custom css
   - `assets/layouts/`: Don't like the default layouts, create your own in this directory
   - `libraries`: files that slidify create. Do not edit the files, copy the file to the `assets` directory and modify it.
* To edit your presentation, edit the `index.Rmd` file using [R Markdown](http://rmarkdown.rstudio.com/)
* To create slides, in the R console run the command


```r
slidify('index.Rmd')``
# View the presentation in a web browser
browserURL('index.html')
```


--- .lehigh


## Slide 3


* Do a Google search for `slidify` to learn more and/or see example slides.

