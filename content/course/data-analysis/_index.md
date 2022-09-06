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

- {{< mention "admin" >}}, Assistant Professor of Sociology 
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

### 0. Prior 

There are several things to do before installation, especially if you are going to use PC (Windows)

0.1. Uninstall `OneDrive` 

    - In recent years, some of laptops (Windows) come with `OneDrive`. 
    - It used to generate errors when installing `R packages.` So far, I could not find any solution for this issue, but unstallation. 
    - Therefore, I recommend you uninstall it before installing R. 
    You can just uninstall it **_Add or remove programs_** like any other program--Please refer to the [link](https://support.microsoft.com/en-us/office/turn-off-disable-or-uninstall-onedrive-f32a17ce-3336-40fe-9c38-6efb09f944b0)
    
    
0.2. Usernames with Latin characters 

    - As you may know, usernames with non-latin characters often generate encoding issues on `R` as in other softwares.
        - Note that non-latin characters indicate Chinese, Japanese and Korean (CJK languages). 
        - It might be okay with installing `R` and `RStudio` but problematic with installing `R packages`.
    - Please change your username into one with latin-characters (e.g. alphabet), if necessary.
    
0.3. Administrative rights

    - You should have administrative rights to install `R`, `RStudio`, and `R packages`
    - Please check whether you have such rights. 
    Otherwise, contact the owner of your laptop. 
    
These are common issues I have encountered in the previous courses. 
The first two things are pretty common for Windows users using Korean (or Chinese)
If you experience any issue while installing `R` and `RStudio`, please check these again. 
Otherwise, please let me know. 
    

### 1. Install R 

In this course, we will use `R` and `RStudio`. 
You need to install `R` first and then `RStudio` later -- not the other way around. 

1.1. Please visit the CRAN (Collective R Archive Network)[^cran] website: <https://cran.r-project.org/>
1.2. Check your OS (Operating Systems) and click on the download link  
    - Windows: "Download R for Windows"
    - macOS: "Download R for macOS" 
1.3. Download installation file
    - Windows: just click the linked text "install R for the first time" and download it
    - macOS: check your macOS version again and choose a corresponding file 
1.4. Double click the downloaded file (probably in your `Downloads` folder). Click "yes" to all prompts. 

1.5. For macOS users, you may need to download and install [XQuartz](https://www.xquartz.org/), depending on your version and systems. 

### 2. Install RStudio

Next, you need to install `RStudio` -- again, install `R` first!
`RStudio` is an integrated development environment (IDE) for R. Simply say, it helps you use `R` better in a more efficient way.  Once you install `R` and `RStudio` successfully, you will mostly use `RStudio` only-- RStudio uses R automatically. -- Think it as `stock market` and `stock trading app`.



2.1. Go to the `RStudio` website and download page <https://www.rstudio.com/products/rstudio/download/#download>

2.2. `RStudio` website detects your OS (macOS or Windows) and shows corresponding program for you. 

2.3. Check and click the download button for your OS 
    - For your information, select "RStudio Desktop" free version. 
    - 
2.4. Double click on the downloaded file and install it on your machine. 

2.5. Start RStudio and check whether everything is okay. 


### 3. Install `tidyverse`

In this course, we will focus on learning `tidyverse` package. 
So, you need to install the `tidyverse` package on your `R` (actually you are going to install it on `RStudio`). 
Think it as installing an mobile app on your smartphone. 

- Please type `install.packages("tidyverse")` on your console and then press 'Enter`. 
- Check whther all the tidyverse packages are installed.



### 4. Install `tinytex`

Depending on course schedule, we may (may not) use `RMarkdown`, which helps us to generate HTML and PDF files from `RStudio`.
In such a process, R utilizes 
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
