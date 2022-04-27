# R 101 conference teaching guide

Thank you for volunteering to teach this one-hour introduction to R at our conference. This teaching guide explains our setup and the material to cover.

The class is one hour long. Every participant will have access to [this directory](https://github.com/ireapps/teaching-guide-R-101/tree/main/Intro-to-R), which includes the necessary R Project file (.Rproj), R Notebook file (.Rmd) and data for the exercises.

It would be a good idea to take a spin through the exercises prior to teaching the session; make sure all the codes runs as written.

## Session description
An introduction to the R programming language and the RStudio app for absolute beginners. This session will cover some necessary terminology, introduce the Tidyverse packages, and go over the basics of data analysis in R. It will prepare participants for moving on to more complex data analysis.

This session is good for: People who are comfortable with sorting, filtering, and grouping data in spreadsheets or database managers.

## Session goals
Attendees should leave with a basic understanding of:
- How to navigate RStudio and use an R Notebook file
- How to assign values to variables
- Basic data types and structures (strings, numbers, vectors)
- Importing data with read_csv
- The arrange(), filter(), summarise() and group_by() functions
- Where to find [instructions for installing R and RStudio on their own machines](https://bit.ly/ire-install-r)
- How to find help when they get stuck

## General approach
I Do, We Do, You Do. Demonstrate a concept, go through it together, then give them plenty of time to experiment on their own while you and your coach walk around and answer questions (see sections marked `*Your Turn!*`). The pace will be slower than you think, and that's OK! It's not the end of the world if you don't get through everything.

Most people who come to this class will have _zero_ experience with programming, so be empathetic and try to remember how frustrating it is to feel lost.

## Class setup
The lab computers will have all the necessary software (R and RStudio) and packages (i.e. Tidyverse) already loaded, along with the class files:
* Intro-to-R.Rproj (double-click this to open RStudio; explain what it is)
* R-101.Rmd (once in RStudio, open this file. It will have all the exercises in it)
* `data` directory (this will have some basic data to import and explore)

Make sure to install tidyverse if you plan to practice or use your own computer: 
`install.packages("tidyverse")`

There are also a couple global settings that need to be tweaked before everything will work smoothly. Make sure you do this if you're using your own computer (the settings on the lab computers will already be set). 

Tools > Global Options > 
1. General > under Workspace, uncheck "Restore .RData..." and for "Save workspace to .RData..." select **Never**
2. R Markdown > "Evaluate chunks in directory:" select **Project**.

## Class outline

### Introduction
Talk through the basics of programming. Have them follow along by double-clicking on the `Introduction-to-R.html` file, which should open up in a browser.

### Main course content
Using `R-101.Rmd`, walk through the concepts slowly, starting with importing tidyverse using the `library()` function.
The exercises will walk through the use of piping and functions and introduce something new in each example, in this order: 
* `read_csv()`
* `<-`
* `%>%`
* `arrange()`
* `arrange(desc())`
* `filter()` (with text)
* `filter() %>% arrange()`
* `filter()` (with numbers)
* `summarise()` with `sum()`
* `summarise()` with `mean()`
* `summarise()` with `n()`
* `filter() %>% summarise()`
* `group_by() %>% summarise()`

Pause frequently to ask if anyone has questions.

Any time you see `*Your Turn!*`, hit the brakes and give everyone a little time to try and answer the question on their own. Then go over the code together.

### Debugging
If you can, find an opportunity when someone has gotten an error and take a couple minutes to walk through basic debugging strategy: Reading the traceback error from bottom to top, strategic Googling, etc.

### If you have extra time at the end
Unlikely! But if you have extra time, ask them some additional questions and give them time to try writing code for the answer, or just let them explore the data on their own.

### Ending the session


