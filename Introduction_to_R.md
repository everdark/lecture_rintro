

<style type="text/css"> 
    .small-code pre code { 
        font-size: 1.3em; 
    } 
</style>

Introduction to R
========================================================
author: Kyle Chung
date: November 28th, 2013 at Trend Micro
width: 1366
height: 768
font-family: 'Consolas'
transition: rotate
transition-speed: fast
incremental: false
navigation: section

Outline
========================================================
+ About me
+ What is R?
+ [Installation and IDE](#/section_ide)
+ [Basic Programming Tips in R](#/section_programming)
    + [Fundamentals](#/section_fundamentals)
    + [Type and Class](#/section_typeclass)
    + [Control Strucure](#/section_control)
    + [Function](#/section_function)
+ [I/O](#/section_io)
+ [Visualization](#/section_visualization)
+ [Final Remarks](#/section_remarks)

About Me
========================================================
left: 25%
![alt MeFunghi.png](Introduction_to_R-figure/everdark.jpg)
<small>illust. by [RedEyeHare](http://redeyehare.tumblr.com/)</small>

[*> My LinkedIn*](http://www.linkedin.com/pub/kyle-chung/59/b34/32)

***

+ Career
    + Now: **SPN Data Correlation, Trend Micro**
    + <small>Former: Data Mining Programmer at Newegg.com</small>
+ Academic Background
    + Master of Economics, NTU
    + Bachelor of International Business, NCCU
        + <small>Double Major Accounting</small>
+ Skills
    + Econometrics, Data Mining, or *something like that*...

And then, about R...
========================================================
type: section

What is R? 
========================================================
type: sub-section
>

R: The most powerful statistical package
========================================================
incremental: true
+ A *general* programming language that is...
    + interpreted
    + designed for statistics
    + with a powerful and active academic community
    + able to run in both interactive and batch mode
    + applicaple to all modern operating systems
    + FREE! (open source)
+ Some useRs consider it *general* due to its high flexibility to develop applications for integration with other infrastructures...
    + ODBC with in-line SQL
    + high-level functions to deal with curl, json, XML...
    + Hadoop integration
    + And many others

Some History
========================================================
incremental: true
+ R is a GNU project based on S language, developed by AT&T (1976)
+ S was then sold (so there is S-PLUS)
+ Okay. That's it.

And why using R?
========================================================
type: sub-section
>

How about other languages?
========================================================
incremental: true
+ Among all over statistical packages such as...
    + **SAS** Extremely expensive with surprisingly little capability.
    + **SPSS** Not programmatically friendly. Not free.
    + **Stata** 
        + Powerful for economics and epidemiology
        + But with limited flexibility and scalability
        + Not free
    + **Matlab** Too fat. Not free.
    + **GAUSS**
        + <small>**G**eneral **A**pparatus for **U**sers to **S**uicide **S**ystematically (*I mean it.*)</small>

Installation
========================================================
type: sub-section
>

Let's Begin!
========================================================
+ For Windows
    + Download and execute the binary
+ For Mac
    + Download and execute the binary
+ For Linux, depending on the distribution...
    + `sudo apt-get install r-base-core`
    + `sudo yum install R-core` (recommend using EPEL)
    + Compile it on your own (don't look at me)
+ R on the cloud
    + [StatAce](http://statace.com/): A startup that allows you to conduct analysis on the cloud

Some Advices
========================================================
+ Choose 64-bit version whenever you can
    + R heavily depends on RAM
    + Some advanced applications only support 64-bit platform, e.g., RHadoop
+ Prefer Linux/Mac over Windows
    + There is a troublesome Unicode encoding issue in Windows not yet solved
        + if you are to analyze data coming from a variety of sources the world over, *you WILL be in trouble*
    + Some useful packages do not have pre-compiled version of or simply cannot run in Windows, e,g, `bigmemory`, `rPython`

IDE for R
========================================================
type: sub-section
id: section_ide
>

RStudio
========================================================
+ http://www.rstudio.com/
+ For all platforms
    + RStudio-Server for Linux server
+ Well integrated with Git
+ Markdown language interface customized for R
    + Slides for this lecture are purely writen in RStudio
+ Module used to develop web app of R based on interactive graphing
+ And yes, **it's FREE!**

IPython Notebook
========================================================
+ http://ipython.org/
+ Generally a Pyhton IDE
+ But you can easily execute R codes
    + try the magic function: `%load_ext rmagic`

Basic Programming Tips in R
========================================================
type: section
id: section_programming

Object-Oriented?
========================================================
type: prompt
> Your role matters!

+ In general, R is an OO language
+ As a software developer:
    + You write your application in OO style
    + You are possibly a contributor to CRAN
+ As a data analyst:
    + You hack into data with procedural or functional programming
    + You only need to know basic concept of OO
+ After all, it's up to you!
    + I personally never write OO-style codes for data analysis purpose

Fundamentals
========================================================
type: sub-section
id: section_fundamentals
>

Environment Setup #1
========================================================











































































































































































```
Error in library(p, character.only = TRUE) : 
  there is no package called 'rCharts'
```
