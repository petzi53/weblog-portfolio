---
title: "Using hugo-academic theme with blogdown (Part 1)"
author: "Peter Baumgartner"
date: '2017-09-04'
slug: tutorial-hugo-academic-theme-with-blogdown-part-1
summary: Part 1 of this tutorial explains how to install the hugo-academic theme on top of blogdown
  and to link it to a new created repository on GitHub.
tags: []
categories: []
---

In this tutorial I will show how to install the R package "blogdown" with the help of the new version of RStudio and how to link your local blogdown-directory to a remote repository on GitHub. But before we actually start with the installation procedure let us define the different ingredients (tools) we are going to use:

## Tools we are going to use

1. [Blogdown](https://bookdown.org/yihui/blogdown/) is an R package for creating static websites with R Markdown. 
2. [R](https://www.r-project.org/about.html) is an integrated suite of open source software facilities for statistical computing and includes tools for data manipulation, calculation and graphical display.
2. [RStudio](https://www.rstudio.com/) is an integrated development environment (IDE) which sits on top of R and facilitates the use of R tremendously.
3. [R Markdown](http://rmarkdown.rstudio.com/) is a file format for making dynamic documents with R. It is based on Markdown (a lightweight markup language with plain text formatting syntax), but it also can contain chunks of embedded R code.
4. [Hugo](https://gohugo.io/) is a popular open-source static website generator.
5. [hugo-academic](https://themes.gohugo.io/academic/) is a theme designed for Hugo to create an academic or personal website. Besides special academic features like sections for publications, projects, teaching it also includes a blog section and supports multilingual usage.
6. [GitHub](https://github.com/) is an Internet hosting service for distributed version control repositories. Is is mainly used for source code management, but it works also with plain text markup languages. GitHub offers all the functionality of Git as well adding its own features.
7. [Git](https://git-scm.com/) is a distributed version control system  for tracking changes in computer files and coordinating work on those files among multiple people.

All these tools are open source and free available. 

## Preliminary preparations: Installing R and RStudio

There are many tutorials to install R and Rstudio. See for instance the video [Installing R and RStudio](https://www.youtube.com/watch?v=cX532N_XLIs). But at the moment the new version of RStudio which facilitats the installation procedure of blogdown is still not released. But you can use all these new features by [downloading the preview release](https://www.rstudio.com/products/rstudio/download/preview/).[^1] As these features will be soon the standard version of RStduio I explain the installation procedure with it.

[^1]: The RStudio version has to be higher than v1.1.28: At the moment (2017-09-04) the new version v1.1.353 is not the standard version and can therefore be downloaded only as preview version. This version works great; I couldn’t find any problems. It has the advantage that you can use some simplification and automated routines during the installation process. 

## Create a website project

After installing a RStudio version greater than 1. v.1.1.28 open a "New Project" in RStudio.

<!-- 
The following r code has to be knitted in order to produce a html/pdf/word file e.g. for bookdown.
The picture is not be seen as static website with hugo
```{r new-project, fig.cap='Create a new project.', fig.align='center', out.width='80%', echo=FALSE} 
 knitr::include_graphics('../../static/img/blogdown-tutorial/01-new-project.png')
``` 
-->

{{< figure src="/img/blogdown-tutorial/01-new-project.png" title="Create new project" >}}


