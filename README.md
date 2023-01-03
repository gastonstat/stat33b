# STAT 33B - Introduction to Advanced Programming in R

- __Description__: The course is designed primarily for those who are already familiar with programming in another language (e.g. Python, C, Java), and want to understand how R works, and for those who already know the basics of R programming and want to gain a more in-depth understanding of the language in order to improve their coding. The focus is on the underlying paradigms in R, such as atomic and non-atomic vectors, functional programming, environments, and object systems (time permitting). The goal of this course is to better understand programming principles in R and to write better R code that capitalizes on the language's design. Topics include (not necessarily covered in the following order): 

    + Data types and data structures in R (e.g. vectors, arrays, lists, data frames)
    + :hammer: Tools for data manipulation
    + :bar_chart: Tools for data visualization
    + :inbox_tray: Data input/output
    + :twisted_rightwards_arrows: Control flow structures (e.g. conditionals, iterations)
    + :pencil: Writing simple functions
    + :loudspeaker: Function calls
    + :bookmark_tabs: Argument matching
    + :heavy_plus_sign: The formula language of R (time permitting)
    + :gift: Building simple R packages

- __Instructor__: [Gaston Sanchez](https://www.gastonsanchez.com)

- __Lecture__: 1 hour of lecture per week

- __Lab__: 1 hour of laboratory per week

- __Assignments__: biweekly HW assignments

- __Exams__: one midterm exam, and final test

- __Texts and Notes__:
    + [Breaking the Ice with R](https://www.gastonsanchez.com/R-ice-breaker)
    + [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)
    + [Rolling Dice](https://www.gastonsanchez.com/R-rolling-dice)
    + [Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)
    + [Handling Strings with R](https://leanpub.com/r4strings)
    + [Pack YouR Code](https://leanpub.com/packyourcode)
    + Prof. Sanchez's slides

- __LMS__: the specific learning resources of a given semester are shared in the Learning Management Sysment (LMS) approved by Campus authorities (e.g. bCourses, Canvas)

- __Policies__:
    + [Lab](https://github.com/gastonstat/course-policies/blob/main/policy-lab.md)
    + [HW](https://github.com/gastonstat/course-policies/blob/main/policy-hw.md)
    + [Email](https://github.com/gastonstat/course-policies/blob/main/policy-email.md)
    + [Academic Integrity](https://github.com/gastonstat/course-policies/blob/main/policy-academic-integrity.md)


-----

## 1. Introduction

:card_index: __ABOUT__:

We begin with the usual review of the course policies, logistics, overall expectations, topics in a nutshell, etc. At the computational level, you'll get introduced to RStudio and R, as well as Markdown and its use in dynamic computational documents (e.g. `Rmd` and `qmd` files).


<br>

:book: __READING__:

- Slides
- [Breaking the Ice with R](https://www.gastonsanchez.com/R-ice-breaker)

<br>

:pencil2: __TOPICS__:

+ __Introduction__
    - About the course
    - First contact with R and RStudio
    - Markdown syntax


-----


## 2. Data Types and Vectors

:card_index: __ABOUT__:

In this week we describe data types and their implementation in R vectors (the most fundamental data object in R).

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Data Types__
    - atomic types (e.g. logical, integer, double, character)
    - coercion
    - vectorization
    - recycling
    - subsetting


-----


## 3. Other Atomic Objects

:card_index: __ABOUT__:

We continue describing more atomic objects such as arrays (N-dimensional objects) and matrices (2-dimensional arrays).

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __More atomic objects__
    - Creation of simple matrices with matrix()
    - How R internally stores matrices
    - Why matrices are atomic objects
    - In what sense a matrix is a 2-dimensional object
    - Matrix subsetting (subscripting, indexing)


-----


## 4. Non-atomic Objects

:card_index: __ABOUT__:

In this week, We continue describing non-atomic objects such as list and data-frames, and we also review how to manipulate (subset) these kind of objects.

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Lists__
    - Manipulation of lists and data frames


-----


## 5. Importing and Exporting Resources

:card_index: __ABOUT__:

In this week, we'll talk about concepts and functions that have to do with so-called input(s)-output(s), or simply put, with importing and exporting operations. For example:

- how to import a data table
- how to export a data table
- how to export a graphic to an image file
- how to export function outputs to external files

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Imports/Exports__
    - `read.table()` and derived functions: e.g. `read.csv()`, `read.delim()`
    - Importing text with `readLines()`
    - Importing code with `soruce()`
    - Exporting output to external files with `sink()`
    - Exporting images with `png()`, `jpeg()`, `pdf()`, etc
    - Mechanism used by R for reading-in data


-----


## 6. First Contact with tidyverse tools (part 1)

:card_index: __ABOUT__:

In addition to learning about the "classic" way to work with data frames, we will briefly touch on an "alternative" approach for working with tables provided by the tidy data framework and the ecosystem of packages known as the `"tidyverse"`: <https://www.tidyverse.org>

This week we start with the tidyverse package `"dplyr"`. Simply put, `"dplyr"` comes with functions to manipulate data-tables (e.g. data-frames, and other 2-dimensional objects) using a modern and syntactic way.

<br>

:book: __READING__:

- [R Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)

<br>

:pencil2: __TOPICS__:

+ __dplyr verbs__
    - `slice()`
    - `filter()`
    - `select()`
    - `arrange()`
    - `group_by()`
    - `summarise()`


-----


## 7. First Contact with tidyverse tools (part 2)

:card_index: __ABOUT__:

Last week we discussed the basics of `"dplyr"`. This week we move on to `"ggplot2"` which is another tidyverse package that allows you to create nice graphics, also following the tidy data framework.

<br>

:book: __READING__:

- [R Tidy Hurricanes](https://www.gastonsanchez.com/R-tidy-hurricanes)

<br>

:pencil2: __TOPICS__:

+ __ggplot verbs__
    - the grammar of graphics
    - geometric objects and visual attributes
    - building a graphic with layers
    - supporting graphical elements


-----


## 8. Conditional "if-else" statements

:card_index: __ABOUT__:

This week we introduce the notion of R expressions, and we provide the syntax used by R to handle if-else statements and related conditionals constructs.

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __If-else statements__
    - R compound expressions and the use of curly braces `{ ... }`
    - Anatomy of an `if-else` statement in R
    - Vectorized if-else function `ifelse()`
    - `switch()` construct
 

-----


## 9. Iterations

:card_index: __ABOUT__:

This week we introduce the syntax used by R to handle iteration constructs such as `for()` loops, `while()` loops, `repeat` loops, and the apply family functions.

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Loops__
    - Anatomy of a `for()` loop in R
    - Anatomy of a `while()` loop in R
    - Anatomy of a `repeat` loop in R
    - `break` statement to stop a loop
    - `next` statement to skip an iteration
    - `apply()` family functions


-----


## 10. Functions

:card_index: __ABOUT__:

This week we review the syntax used by R for writing functions. We also take a look at auxiliary functions such as `return()`, `stop()`, and `warning()`

<br>

:book: __READING__:

- [R Coding Basics](https://www.gastonsanchez.com/R-coding-basics)

<br>

:pencil2: __TOPICS__:

+ __Functions__
    - Main parts of a function (i.e. anatomy of a function)
    - Examples for creating a function
    - Difference between positional arguments, and named arguments
    - Binary opeartor functions

 
-----


## 11. Functions and Scoping

:card_index: __ABOUT__:

This week we review more technical aspects of functions in R. Specifically, we will focus on the scoping mechanisms used by R to find the value of a variable.

<br>

:book: __READING__:

- Slides

<br>

:pencil2: __TOPICS__:

+ __Environments__
    - What is an environment?
    - Creating environments
    - Types of environments
    - The search list
+ __Scoping principles__
    - Name maksing
    - Functions vs Variables
    - Fresh start
    - Dynamic lookup


-----


## 12. Performance and Profiling

:card_index: __ABOUT__:

This week we review more underlying principles that have to do with performance in R.

<br>

:book: __READING__:

- Slides

<br>

:pencil2: __TOPICS__:

+ __R's behavior__
    - R's motto
    - Copy-on-modify policy
    - What things make R slow
+ __Performance__
    - Measuring performance in a "quick-and-dirty" way with `system.time()`
    - Profiling code with `Rprof()` and `"profvis"`
    - Alternative way to measure performance with `"microbenchmark"`
 

-----


## 13. Packaging (part 1)

:card_index: __ABOUT__:

This week we review the anatomy of an R package.

<br>

:book: __READING__:

- Slides

<br>

:pencil2: __TOPICS__:

+ __Anatomy of an R package__
    - `DESCRIPTION` file
    - `NAMESPACE` file
    - `R/` folder
    - `man/` folder
    - `Roxygen` comments and `Rd` files
 

-----


## 14. Packaging (part 2)

:card_index: __ABOUT__:

This week we go through the first steps for creating a simple R package.

<br>

:book: __READING__:

- Slides

<br>

:pencil2: __TOPICS__:

+ __Building an R package__
    - `devtools` functions
    - Create `Rd` files with `document()`
    - Check content of `Rd` files with `check_man()`
    - Build a bundle with `build()`
    - Install a package locally with `install()`
