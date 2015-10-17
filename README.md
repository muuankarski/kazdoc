### Overview

The **kazdoc** package includes a set of [R Markdown](http://rmarkdown.rstudio.com) templates that enable authoring of R related publications commonly produced within rstatscon. Available templates include:

- kaz_plain

<!--

The **rticles** package includes a set of [R Markdown](http://rmarkdown.rstudio.com) templates that enable authoring of R related journal and conference submissions, and creating e-books. Available templates include:

- [Tuftish e-book] e-books formatted based on the style of Edward R. Tufte and Richard Feynman

- [JSS](http://www.jstatsoft.org/) articles

- [R Journal](http://journal.r-project.org/) articles

- [useR](http://user2014.stat.ucla.edu/) conference abstracts

- [Public Library of Science (PLoS)](http://www.plos.org/) articles

- [CTeX](http://ctex.org) documents

- [ACS](http://pubs.acs.org) articles

Under the hood, LaTeX templates are used to ensure that documents conform precisely to submission standards. At the same time, composition and formatting can be done using lightweight [markdown](http://rmarkdown.rstudio.com/authoring_basics.html) syntax, and R code and its output can be seamlessly included using [knitr](http://yihui.name/knitr/).

Using **rticles** has some prerequisites which are described below. You can get most of these pre-requisites automatically by installing the latest preview release of RStudio (instructions for using **rticles** without RStudio are also provided).

-->

### Using faodoc from RStudio

To use **kazdoc** from RStudio:

1) Install the latest [RStudio](http://www.rstudio.com/products/rstudio/download/).

2) Install the **kazdoc** package: 

```S
devtools::install_github("muuankarski/kazdoc")
```

3) Use the **New R Markdown** dialog to create an article from one of the templates:

![New R Markdown](http://rmarkdown.rstudio.com/images/new_r_markdown.png)
    
    
### Using faodoc outside of RStudio

1) Install [pandoc](http://johnmacfarlane.net/pandoc/) using the [instructions for your platform](https://github.com/rstudio/rmarkdown/blob/master/PANDOC.md).

2) Install the **rmarkdown** and **kazdoc** packages:

```S
devtools::install_github(c("rstudio/rmarkdown", "muuankarski/kazdoc"))
```
    
3) Use the `rmarkdown::draft` function to create articles:

```S
rmarkdown::draft("MyAbstract.Rmd", template = "kaz_plain", package = "kazdoc")
```

