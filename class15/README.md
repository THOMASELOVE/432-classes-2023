# 432 Class 15: 2023-03-07

[Main Website](https://thomaselove.github.io/432-2023/) | [Calendar](https://thomaselove.github.io/432-2023/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2023/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | PDF | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
15 | 2023-03-07 | **[Slides 15 (and 16)](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides15.pdf)** | **[Code 15 (and 16)](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides15.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

![](carr_2021-03-26.png)

## Announcements

1. There is a [Minute Paper after Class 15](https://bit.ly/432-2023-minute-15). Please complete it by noon Wednesday (2023-03-08).
2. The Lab 5 Answer Sketch and Grading Rubric is now available in the Answer Sketches subfolder in our Shared Drive.
3. Bonus [Lab X](https://thomaselove.github.io/432-2023/labX.html) now exists. Please take a look.
4. We've pinned a prompt about "How To Be A Modern Scientist (Discussion 2)" to Campuswire, and will again award class participation credit to people who respond over the next two weeks.
5. Those of you wanting me to review some aspect of the grading of your Quiz 1, please send me an email by 9 AM tomorrow (Wednesday). I will review them all tomorrow, including those I have already received from Aman, Seth and Tian.
6. I have updated Chapter 26 of the [Course Notes](https://thomaselove.github.io/432-notes/) to fix an error in the list of methods discussed in the chapter, and Chapters 29 and 30 to fix broken links. I also fixed a typo in the [Lab 6 instructions](https://thomaselove.github.io/432-2023/lab6.html).
7. Remember that we do not have class **next** week, thanks to Spring Break.
    - Specifically, after our class 16 this Thursday 2023-03-09, the next class (Class 17) will be Tuesday 2023-03-21.
    - No TA office hours will be held beginning Friday 2023-03-10 through Friday 2023-03-17. TA office hours will resume on Saturday 2023-03-18 after this break.
    - Dr. Love will answer his email approximately once per day for 432 matters, and will also address questions posted to Campuswire approximately once per day between 2023-03-10 and 2023-03-19.
8. Remember that your Project A portfolio is due the Monday after Spring Break, 2023-03-20, at 9 PM.
    - The [Project A portfolio](https://thomaselove.github.io/432-2023/projA.html#the-project-a-portfolio) consists of these four elements:
        1. a Quarto (.qmd) file containing containing one unnumbered, and 13 numbered sections (10 of which come from the Plan.)
        2. an HTML result of applying the Quarto “portfolio” file to your data
        3. a copy of your tidy data and link to where Professor Love can obtain the raw data freely
        4. a video (not to exceed 5 minutes) presenting one of your key project results (see the [Presentation materials in the instructions](https://thomaselove.github.io/432-2023/projA.html#the-presentation))
    - I have posted [several Project A tips below](#a-few-project-a-tips). 
    - All 46 project A plans [have been accepted](https://github.com/THOMASELOVE/432-classes-2023/blob/main/projectA/plans.md).

----

# A Few Project A Tips

- The TAs (first) and Dr. Love (second) will inspect your Quarto and HTML files, and perhaps your data.
- Dr. Love (alone) will watch your videos. 
- Dr. Love will decide your project A grade. 
- This means the videos will have more to do with your final score than you might think.

## Why I use `read_csv()` all the time, and never use `read.csv()` anymore

1. `read_csv()` is much faster than `read.csv()`, 
2. `read_csv()` provides a progress meter and a compact method for specifying column types,
3. `read_csv()` will read compressed files automatically,
4. `read_csv()` automatically creates a tibble, and
5. `read_csv()` allows me to speed the process of debugging by providing much more useful error messages about which rows are problematic, especially when the error is non-fatal.

- For more details, see the [Data import section of R for Data Science](https://r4ds.hadley.nz/data-import.html).
- From Josh Gonzales at Medium: [read_csv(): The Best Way to import CSV data into R](https://medium.com/r-tutorials/r-functions-daily-read-csv-3c418c25cba4)

## What should I do if I have a problem with Normality in my linear model (Project A)?

1. Not all problems can be fixed with power transformations and non-linear terms.
2. You should describe what the residual plots show, accurately.
3. If there is a problem with the residual plots, use that fact in making a decision about which model to select as your final model. 
4. If you have to select a final model with residual plot problems, describe how those problems might affect your conclusions.

## Exploding Coefficients and Problems in Logistic Regression

Sometimes, we see people fitting models to predict a binary outcome using a predictor which completely determines that outcome (for example, if predictor > 12, then outcome is always no, or if predictor = "Yes" then outcome is always no.)

Take a look at [this toy example with explosive coefficients](https://rpubs.com/TELOVE/explosion_logistic_432) to see one way in which this problem can emerge and what to do about it.

## Some Common Problems You Can Fix in your Project A

1. Sometimes, we see people failing to drop levels of a categorical predictor after combining levels. Use the `droplevels()` command.
2. Sometimes, we see people fitting restricted cubic splines or polynomials either to categorical predictors or to quantitative predictors with just a few observed values.
3. Remember that it's perfectly fine to add fewer than the maximum additional degrees of freedom beyond the main effects model [if necessary, so long as you include at least one non-linear term](https://thomaselove.github.io/432-2023/projA.html#new-section-8.-linear-regression-analyses)
4. Suppose you decide to create a decision rule for a logistic regression model. If 10% of your observations are "Yes" on your binary outcome, and 90% are "No", then use a .fitted value of something like 0.1 as your decision rule. Don't use 50% unless your observations are split pretty close to 50-50 between your two categories for your binary outcome.
5. When you build a plot of the ROC curve for your final model, be sure it provides the same C statistic value as you get from the `lrm` fit to the data, and that you also provide the validation-adjusted C statistic estimate for that model.
6. Something we've seen **a lot** in looking at Quarto files people have sent is the failure to include a blank line **before and after** every **heading and subheading**, and **every block of code**.
7. Don't name the file `projectAproposal.Rmd` when it's not your proposal. A good generic name would be `2023-03-07_432_projA.Rmd` or `432projectA_2023-03-07.Rmd` assuming it's the version from that date (2023-03-07).
8. Be sure to run the spell-check, and ideally, have someone else read through your work.
9. We hate scrolling windows in HTML output caused by code that runs too long on one line. Use the ENTER key liberally to help avoid this problem, and check your HTML to see if it is happening.
10. Make sure your headings are in an appropriate order, and that you have 13 main sections in your Project, as laid out in the sample project. Check your HTML to make sure the headings make sense, for instance, `10`, then `10.1`, then `10.1.1.` is OK, but `10`, then `10.0.1` isn't OK.
11. If you're loading a package not on our [R packages list](https://thomaselove.github.io/432-2023/software.html#r-packages-to-install), then you should definitely indicate why you're doing this at the top of your work as you load it in a short comment. Also, don't load elements of [the core `tidyverse`](https://www.tidyverse.org/packages/) separately: load them with `tidyverse` only.

---

## This Week's Agenda: Regression on Count Outcomes

- Today's slides will be used both today and Thursday (in Class 16).

This week, we'll be presenting some key ideas on fitting models for count outcomes. Counts are discrete (rather than continuous) and counts are typically integers (0, 1, 2, 3 and so on) and cannot be made more precise. Relevant materials are available in Chapters 24-26 of the [Course Notes](https://thomaselove.github.io/432-notes/). 

Methods we will touch on this week include Poisson regression and negative binomial regression, along with augmentations of these two approaches to inflate the number of zeros predicted, and also "hurdle" versions which specify one process for zero counts and another for positive counts. In Chapters 24-26, we discuss all of these, as well as another approach, called a tobit (or censored) regression model.

![](ghement.png)

Here's [a link to the start of the "tweetorial"](https://twitter.com/IsabellaGhement/status/1363957122787024901) on some key practical aspects of understanding Poisson regression models.

## On Rootograms

To install the [countreg package from R-Forge](https://r-forge.r-project.org/R/?group_id=522) in R, you will need to use the following command (note that the package is not available on CRAN):

```
install.packages("countreg", repos="http://R-Forge.R-project.org")
```

For more on rootograms, check out Kleiber C Zeileis A [Visualizing Count Data Regressions Using Rootograms](rootograms_2016.pdf) from *The American Statistician* 2016.

----

## What You Should Be Working On

1. [Minute Paper after Class 15](https://bit.ly/432-2023-minute-15), due Wednesday 2023-03-08 at noon.
2. [Project A Portfolio](https://thomaselove.github.io/432-2023/projA.html), due Monday 2023-03-20 at 9 PM.
