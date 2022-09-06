---
title: "SOC3035 DATA ANALYSIS"
linkTitle: DATA ANALYSIS
date: "2022-09-01"
summary: Course Overview of Data Analysis 
type: book
tags: current
---

{{< figure src="featured.jpg" >}}

{{< toc hide_on="xl" >}}


{{% callout note %}}
Course materials (slides) and assignment will be posted on *HY-ON*, an LMS at Hanyng University.
{{% /callout %}}


## **Course Information** 

- Class hours: Wed 1~4pm 
- Class room: 303 Social Sciences 

- {{< mention "admin" >}}, Assistant Professor of Sociology 
- email: samyoo@hanyang.ac.kr
- Office: 408 Social Sciences


### Course description

This course is an introduction to the field of data analysis and visualization in sociology. It will guide you how to manage, analyze, and visualize quantitative data from diverse topics in sociology. This course is designed to learn the basic knowledge and usages of statistical software, such as Excel and R, in data wrangling, data analysis, and visualization. Basic computer skills are essential to successfully complete this course, though intermediate or advanced computer skills are preferred.

### Required prerequisite

- CUL2004: Invitation to Sociology, or equivalent 
- SOC2002: Social Statistics, or equivalent

Otherwise, please contact the instructor before registering.

### Course objectives

Upon successful completion of this course, students will  
- Understand how to manage, analyze, and interpret quantitative data 
- Have practical knowledge and senses of how to present quantitative data through effective graphs and figures.
- Gain on hands-on skills and experience with R and RStudio (especially tidyverse packages).

### Course syllabus 

Please check {{< staticref "uploads/DataAnalysis2022_syllabus.pdf" "newtab" >}}Course syllabus{{< /staticref >}}.

### Course slides 



## Installation

### 0. Prior 

There are several things to do before installation, especially if you are going to use PC (Windows)

0.1. Uninstall `OneDrive` 

- In recent years, some of laptops (Windows) come with `OneDrive`.   
    
- It used to generate errors when installing `R packages.` So far, I could not find any solution for this issue, but unstallation. 
    
- Therefore, I recommend you uninstall it before installing R. 
    
You can just uninstall it **_Add or remove programs_** like any other program -- Please refer to the [link](https://support.microsoft.com/en-us/office/turn-off-disable-or-uninstall-onedrive-f32a17ce-3336-40fe-9c38-6efb09f944b0)
For those who want to maintain `OneDrive`, please visit the webpage below and then follow instructions: [here](https://medium.com/@ValidScience/how-to-fix-rstudios-package-installation-on-windows-10-c1e602bf3a1f) 
    
    
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

1.1. Please visit the CRAN (Collective R Archive Network) website: <https://cran.r-project.org/>

1.2. Check your OS (Operating Systems) and click on the download link  

- Windows: click on "Download R for Windows"  
    
- macOS: click on "Download R for macOS"   
    
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

- For your information, select "RStudio Desktop" free version (if necessary). 
 
2.4. Double click on the downloaded file and install it on your machine. 

2.5. Start RStudio and check whether everything is okay. 


### 3. Install `tidyverse`

In this course, we will focus on learning `tidyverse` package. 
So, you need to install the `tidyverse` package on your `R` (actually you are going to install it on `RStudio`). 
Think it as installing an mobile app on your smartphone. 

3.1. Please type `install.packages("tidyverse")` on your console and then press 'Enter`. 

3.2. Check whther all the tidyverse packages are installed.



### 4. Install `tinytex`

Depending on course schedule, we may (may not) use `RMarkdown`, which helps us to generate HTML and PDF files from `RStudio`.
In such a process, R uses `LaTeX`, an open-source special scientific typesetting program. There are several software of `LaTeX`, such as `TexLive` and `MikTex`. However, those are independent software with heavy volume. `TinyTex` is another R package of a light LaTex program. 

4.1. type and run `install.packages("tinytex")` in the console.

4.2. Run `tinytex::install_tinytex()` in the console.

4.3. R will download and install everything you need.



### 5. Optional, but recommended:

5.1. Install `git` [https://git-scm.com/downloads](https://git-scm.com/downloads) 

- No other separate `git` program is required. We'll just use it from `Rstudio` a bit.

5.2. sign up and open your account at `github.com`

### More 

Here are some links that cover the topic of installation and update of R on different OSs. 

* Install R and RStuido for macOS & Windows
    - [MacOS users](https://www.reed.edu/data-at-reed/software/R/r_studio.html) 
    - [PC (Windows) users](https://www.reed.edu/data-at-reed/software/R/r_studio_pc.html)

* Update R, R packages and R studio 
[here](https://bootstrappers.umassmed.edu/bootstrappers-courses/courses/rCourse/Additional_Resources/Updating_R.html)

* Tutorial on updating R on Windows with screenshots
[here](https://www.r-statistics.com/2015/06/a-step-by-step-screenshots-tutorial-for-upgrading-r-on-windows/)

* Video guide for installing R and RStudio for Windows
[here](https://www.youtube.com/watch?v=NZxSA80lF1I&ab_channel=TechDecodeTutorials)

* RTools guide for Windows:
[here](https://www.youtube.com/watch?v=FXWLR2DGgI8&t=34s)
