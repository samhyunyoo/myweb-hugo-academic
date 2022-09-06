---
title: "SOC3035 DATA ANALYSIS"
linkTitle: Data Science
date: "2022-09-01"
summary: Course Overview of Data Analysis 
type: book
tags: current
---

{{< figure src="featured.jpg" >}}

{{< toc hide_on="xl" >}}


## Course Information 

- Class hours: Wed 1~4pm 
- Class room: 303 Social Sciences 

- Sam Hyun Yoo (Ph.D.), Assistant Professor of Sociology 
- email: samyoo@hanyang.ac.kr
- Office: 408 Social Sciences


#### Course description

This course is an introduction to the field of data analysis and visualization in sociology. It will guide you how to manage, analyze, and visualize quantitative data from diverse topics in sociology. This course is designed to learn the basic knowledge and usages of statistical software, such as Excel and R, in data wrangling, data analysis, and visualization. Basic computer skills are essential to successfully complete this course, though intermediate or advanced computer skills are preferred.

#### Required prerequisite

- CUL2004: Invitation to Sociology, or equivalent 
- SOC2002: Social Statistics, or equivalent

Otherwise, please contact the instructor before registering.

#### Course objectives

Upon successful completion of this course, students will  
- Understand how to manage, analyze, and interpret quantitative data 
- Have practical knowledge and senses of how to present quantitative data through effective graphs and figures.
- Gain on hands-on skills and experience with R and RStudio (especially tidyverse packages).

## Installation

### 0. Things to check before installation 

There are several things to do before installation, especially if you are going to use PC (Windows)

1. Uninstall `OneDrive` 

    - In recent years, some of laptops (Windows) come with `OneDrive`. It used to generate errors when users install `R packages.` So far, I have not known any solution for this issue. Therefore, I recommend to uninstall it before installing R. You can just uninstall it **_Add or remove programs_** like any other program.
    - Please check the [link](https://support.microsoft.com/en-us/office/turn-off-disable-or-uninstall-onedrive-f32a17ce-3336-40fe-9c38-6efb09f944b0)

2. Change your username (Windows account) into new one with Latin characters 



    
    
    
    

### 1. Install R 

In this course, we will use `R` and `RStudio`. 
You need to install `R` first and then `RStudio` later -- not the other way around. 


1. Please visit the CRAN (Collective R Archive Network)[^cran] website: <https://cran.r-project.org/>
2. Check your OS (Operating Systems) and click on the download link  
    - Windows: "Download R for Windows"
    - macOS: "Download R for macOS" 
3. Download installation file
    - Windows: just click the linked text "install R for the first time" and download it
    - macOS: check your macOS version again and choose a corresponding file 
4. Double click the downloaded file (probably in your `Downloads` folder). Click "yes" to all prompts. 

5. For macOS users, you may need to download and install [XQuartz](https://www.xquartz.org/), depending on your version and systems. 

### 2. Install RStudio

Next, you need to install RStudio, the nicer graphical user interface (GUI) for R (the dashboard). Once R and RStudio are both installed, you can ignore R and only use RStudio. RStudio will use R automatically and you won't ever have to interact with it directly.

1. Go to the free download location on RStudio's website: <https://www.rstudio.com/products/rstudio/download/#download>
2. The website should automatically detect your operating system (macOS or Windows) and show a big download button for it:

    <img src="/img/install/install-r-rstudio1.png" width="50%" />
    
    If not, scroll down a little to the large table and choose the version of RStudio that matches your operating system.

    <img src="/img/install/install-r-rstudio2.png" width="100%" />

3. Double click on the downloaded file (again, check your `Downloads` folder). Click yes through all the prompts to install like any other program.

Double click on RStudio to run it (check your applications folder or start menu).


### Install `tidyverse`

R packages are easy to install with RStudio. Select the packages panel, click on "Install," type the name of the package you want to install, and press enter.

<img src="/img/install/install-r-package-panel.png" width="40%" />

This can sometimes be tedious when you're installing lots of packages, though. [The tidyverse](https://www.tidyverse.org/), for instance, consists of dozens of packages (including **ggplot2**) that all work together. Rather than install each individually, you can install a single magical package and get them all at the same time.

Go to the packages panel in RStudio, click on "Install," type "tidyverse", and press enter. You'll see a bunch of output in the RStudio console as all the tidyverse packages are installed.

<img src="/img/install/install-r-tidyverse.png" width="60%" />

Notice also that RStudio will generate a line of code for you and run it: `install.packages("tidyverse")`. You can also just paste and run this instead of using the packages panel.


### Install `tinytex`

When you knit to PDF, R uses a special scientific typesetting program named LaTeX (pronounced "lay-tek" or "lah-tex"; for goofy nerdy reasons, the x is technically the "ch" sound in "Bach", but most people just say it as "k"—saying "layteks" is frowned on for whatever reason).

LaTeX is neat and makes pretty documents, but it's a huge program—[the macOS version, for instance, is nearly 4 GB](https://tug.org/mactex/mactex-download.html)! To make life easier, there's [an R package named **tinytex**](https://yihui.org/tinytex/) that installs a minimal LaTeX program and that automatically deals with differences between macOS and Windows.

Here's how to install **tinytex** so you can knit to pretty PDFs:

1. Use the Packages in panel in RStudio to install **tinytex** like you did above with **tidyverse**. Alternatively, run `install.packages("tinytex")` in the console.
2. Run `tinytex::install_tinytex()` in the console.
3. Wait for a bit while R downloads and installs everything you need.
4. The end! You should now be able to knit to PDF.


* Rstudio Desktop, preview version [https://www.rstudio.com/products/rstudio/download/preview/](https://www.rstudio.com/products/rstudio/download/preview/)
Installing this will automatically install the latest `R` version `4.1.0`, which we need.

optional, but recommended to install:
* `git` [https://git-scm.com/downloads]()https://git-scm.com/downloads No need for a separate `git` program. We'll just use it from `Rstudio` a bit.
* `latex` [https://www.latex-project.org/get/](https://www.latex-project.org/get/)  Alternatively we can install it straight from `R` using the `tinytex` package.

## Further resources that might help installation:

Here are some links that exhaustively cover the topic of installation and update of R on different platforms.

* Install R and tidyverse for Mac, Windows. With some update guides
[https://uvastatlab.github.io/phdplus/installR.html](https://uvastatlab.github.io/phdplus/installR.html)
[https://courses.edx.org/courses/UTAustinX/UT.7.01x/3T2014/56c5437b88fa43cf828bff5371c6a924/](https://courses.edx.org/courses/UTAustinX/UT.7.01x/3T2014/56c5437b88fa43cf828bff5371c6a924/)

* Update R, R packages and R studio on different platforms 
[https://bootstrappers.umassmed.edu/bootstrappers-courses/courses/rCourse/Additional_Resources/Updating_R.html](https://bootstrappers.umassmed.edu/bootstrappers-courses/courses/rCourse/Additional_Resources/Updating_R.html)

* Full tutorial for updating R on Windows with screenshots
[https://www.r-statistics.com/2015/06/a-step-by-step-screenshots-tutorial-for-upgrading-r-on-windows/](https://www.r-statistics.com/2015/06/a-step-by-step-screenshots-tutorial-for-upgrading-r-on-windows/)

Installation guide for r and rstudio for Windows
[https://www.youtube.com/watch?v=NZxSA80lF1I&ab_channel=TechDecodeTutorials](https://www.youtube.com/watch?v=NZxSA80lF1I&ab_channel=TechDecodeTutorials)

RTools guide, for those still having problems on Windows:
[https://www.youtube.com/watch?v=FXWLR2DGgI8&t=34s](https://www.youtube.com/watch?v=FXWLR2DGgI8&t=34s)

👋❤️👉 📚 💬 🐦 💡



## What you will learn

- Fundamental {{<hl>}}Python programming skills{{</hl>}}
- {{<hl>}}Statistical concepts{{</hl>}} and how to apply them in practice
- Gain experience with the {{<hl>}}Scikit{{</hl>}}, including data visualization with {{<hl>}}Plotly{{</hl>}} and data wrangling with {{<hl>}}Pandas{{</hl>}}

## Program overview

The demand for skilled data science practitioners is rapidly growing. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi.

## Courses in this program

{{< list_children >}}

## Meet your instructor

{{< mention "admin" >}}

## FAQs

{{< spoiler text="Are there prerequisites?" >}}
Yes, there are. 1) Any introductory course to sociology (ex., Introduction to Sociology) and 2) Any statistics at undergraduate levels (ex., Social Statistics) 
{{< /spoiler >}}

{{< spoiler text="How often do the courses run?" >}}
Once a week, three credits
{{< /spoiler >}}

{{< cta cta_text="Begin the course" cta_link="hanyang.ac.kr" >}}
