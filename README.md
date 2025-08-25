# Emory IBS 519 Guest Lectures: Fall 2025
{:.no_toc}

-----

by Melinda Higgins, PhD; [https://melindahiggins.netlify.app/](https://melindahiggins.netlify.app/)

-----

* TOC 1
{:toc}

-----

# Melinda's First Lecture: Intro to R, RStudio and Rmarkdown

## This class will cover:

* Explore RStudio environment
    - command line
    - R scripts
    - packages
    - getting help 
* [RStudio Education](https://education.rstudio.com/)
* [R markdown intro (brief)](https://rmarkdown.rstudio.com/) 
* Importing & viewing data
    - [abalone dataset](https://archive.ics.uci.edu/ml/datasets/abalone)
    - `str()`, `dim()`, `head()`, `tail()` functions
* Data types - classes of variables
    - strings
    - integers
    - numeric
    - logical
    - factors (brief intro)

## Materials

* [Posit Cloud](https://posit.cloud/) Project "IBS_519_mhiggins_RRStudioIntro"
    - three R scripts
    - and simple Rmarkdown report to get started
    - stored on [Github](https://github.com/melindahiggins2000/IBS_519_wk1_lecture02_mhiggins)
* Optional: [Intro to R and RStudio](https://melindahiggins2000.github.io/CDC_Rworkshop_April2022/CDCRworkshop_April2022_Module01.html#1)
* [Getting Started with Packages](https://melindahiggins2000.github.io/CDC_Rworkshop_April2022/CDCRworkshop_April2022_Module02.html#1)
* Optional: [Introduction to R Objects](https://melindahiggins2000.github.io/N741_Spring2021_lesson04_dataWranglingDplyr/N741_IntroductionToRObjects_mkh.html#1)
* Optional: [R Objects - Brief Overview of Factors](https://melindahiggins2000.github.io/N741_Spring2021_lesson04_dataWranglingDplyr/N741_RObjectsFactors_mkh.html#1)
* Optional: [Intro to ggplot2 (i.e. week 2)](https://melindahiggins2000.github.io/CDC_Rworkshop_April2022/CDCRworkshop_April2022_Module03.html#1)
* Optional: 
    - [Intro to Data Wrangling with dplyr](https://melindahiggins2000.github.io/CDC_Rworkshop_April2022/CDCRworkshop_April2022_Module04.html#1)

-----

# Melinda's Second Lecture: Data Exploration and Wrangling (with dplyr)

## This class will cover:

* Data exploration
    - numerical exploration
        - `summary()` function
        - `describe()` function from [`Hmisc` package](https://hbiostat.org/R/Hmisc/)
        - `describe()` function from [`pysch` package](https://cran.r-project.org/web/packages/psych/index.html)
    - graphical exploration
        - histograms
        - scatterplots
        - learn more at:
            - [R Graphics Cookbook](https://r-graphics.org/)
            - [Cookbook for R, graphics codes for book](http://www.cookbook-r.com/Graphs/)
            - [R Graph Gallery](https://r-graph-gallery.com/)
* more with the `abalone` dataset
* Tidyverse - [`dyplr` package](https://dplyr.tidyverse.org/index.html)
    - glimpse
    - select
    - filter (explore and clean)
    - arrange
    - mutate (making new variables)
    - rename
    - summarise
    - group_by
    
## Materials

* [Posit Cloud](https://posit.cloud/) Project - in class exercises
  - see "IBS_519_mhiggins_DataWrangling" on [Posit.cloud](https://posit.cloud/)
  - also see [Github repository](https://github.com/melindahiggins2000/IBS_519_wk3_lecture06_mhiggins)
* [Posit Cloud](https://posit.cloud/) Project - Homework 3
  - see "Assignment3_HW3_DataWrangling_Cleaning" on [Posit Cloud](https://posit.cloud/)
  - also see [Github repository](https://github.com/melindahiggins2000/IBS_519_Fall2023_HW3)

-----

# Melinda's Third Lecture: Reproducible Research and RMarkdown

## Today's class will cover:

* Make your life easier with [Rmarkdown](https://rmarkdown.rstudio.com/)
    - [Rmarkdown Output Options](https://rmarkdown.rstudio.com/gallery.html)
    - [RMarkdown Formats](https://rmarkdown.rstudio.com/formats.html)
* Writing a step-by-step analysis report 
    - make DOCX and HTML reports (PDF optional)
* Using parameters - automate your work - learn more at:
    - [RMarkdown: Definitive Guide, Ch 15](https://bookdown.org/yihui/rmarkdown/parameterized-reports.html)
    - [RMarkdown Cookbook: Ch 17.4](https://bookdown.org/yihui/rmarkdown-cookbook/parameterized-reports.html)
    
* Making other "Rmarkdown" formats
    - see [Rmarkdown Galley](https://rmarkdown.rstudio.com/gallery.html)
    - Documents (HTML, DOC and PDF - see notes below)
    - Slides (HTML slidy and ioslides; PDF Beamer; and Microsoft Powerpoint PPT)
    - and other templates - see RMarkdown Gallery to learn more
* more on making PDF documents:
    - PDF requires some version of LaTeX - easiest is installing the `tinytex` package
        - see [https://yihui.org/tinytex/](https://yihui.org/tinytex/)
        - after installing the `tinytex` package, you still have to run `tinytex::install_tinytex()` to actually install the tinytex program with all of the LaTeX packages.
        - Learn more about LaTeX at:
            * [https://www.latex-project.org/](https://www.latex-project.org/)
            * [https://www.overleaf.com/](https://www.overleaf.com/)


## Materials for Rmarkdown Lecture Exercises

[Posit Cloud](https://posit.cloud/) Project "IBS_519_mhiggins_Rmarkdown" - files explained:

This project is also posted in Github at [https://github.com/melindahiggins2000/IBS_519_wk4_lecture08_mhiggins](https://github.com/melindahiggins2000/IBS_519_wk4_lecture08_mhiggins)

### Main Examples Today:

Files:

* 01_Basic_RmarkdownReport.Rmd
* 02_Default_RmarkdownTemplate.Rmd
    - make reports (HTML, DOCX and PDF)
    - make slides (slidy, ioslides, beamer and PPT)
* 03_AbaloneReport_simple.Rmd
* 04_AbaloneReport_paramTemplate.Rmd
* 05_AbaloneReport_paramInYAML.Rmd
* 06_AbaloneReport_param_UserInput.Rmd

Packages used in main examples today:

* `tidyverse` (includes `readr`, `dplyr`, `ggplot2`)
* `knitr`
* `printr`
* `rmarkdown`
* `purrr`
* `gtsummary`

### IF TIME - optional demos:

Files:

* rmdformats_readthedown.Rmd
* flexdashboard.Rmd
* EDA_tools.Rmd

Packages needed:

* For EDA_tools.Rmd
    - `skimr`
    - `summarytools`
* For rmdformats_readthedown.Rmd
    - `rmdformats`
* For flexdashboard.Rmd
    - `flexdashboard`

### Follow-up from Second Lecture - sorting/arrange

* review the `order_sort_arrange.R` scipt

### More resources:

* [`knitr` package](https://cran.r-project.org/web/packages/knitr/index.html)
* [`printr` package](https://cran.r-project.org/web/packages/printr/)

-----

# R/RStudio Helpful Resources

* [Download: R from CRAN](https://cran.r-project.org/)
    - This is where you can download the R language software for FREE for your own computer.
    - Choose your operating system (Mac OS or Windows or Linux/Unix)
    - NOTE: For Windows, you should also download and install [Rtools](https://cran.r-project.org/bin/windows/) - this is technically optional, but is useful to have. Make sure to download the one for your R version.
    
* [Download: RStudio IDE Desktop](https://www.rstudio.com/products/rstudio/download/#download)
    - Note: Windows is listed at the top - just scroll down to see the installer for the Mac OS as well. There are also installers for the versions of Linux/Unix.

* [RStudio/Posit Education](https://education.rstudio.com/)
* [Posit Cloud Getting Started](https://docs.posit.co/cloud/get_started/)
* [Posit Cloud Recipes](https://posit.cloud/learn/recipes)
* [** Quick-R **](https://www.statmethods.net/)
* [Rmarkdown Tutorial](https://rmarkdown.rstudio.com/lesson-1.html)
* [Quarto](https://quarto.org/) - the "next" evolution of Rmarkdown
* [tidyverse](https://www.tidyverse.org/)

* [Datacamp](https://www.datacamp.com/)
* [R for SAS Users - My Datacamp Course](https://www.datacamp.com/courses/r-for-sas-users)
* [Coursera](https://www.coursera.org/)
* [Reproducible Templates for Analysis and Dissemination - My Coursera Course](https://www.coursera.org/learn/reproducible-templates-analysis)
* [Emory N741](https://melindahiggins2000.github.io/N741bigdata/)
* [Emory N736](https://melindahiggins2000.github.io/N736/)
* [Book: Statistical Inference via Data Science](https://moderndive.com/)
* [Book: The Epidemiologist R Handbook](https://epirhandbook.com/en/index.html)
* [Book/Course: Stat 545](https://stat545.com/)

