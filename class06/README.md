# 432 Class 06: 2023-02-02

[Main Website](https://thomaselove.github.io/432-2023/) | [Calendar](https://thomaselove.github.io/432-2023/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2023/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

![](https://imgs.xkcd.com/comics/data_point.png) <https://xkcd.com/2713> 

## Today's Slides

Class | Date | PDF | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
06 | 2023-02-02 | **[Slides 06](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides06.pdf)** | **[Code 06](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides06.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

- The PDF link provides the version of the slides that I suggest you focus on during class.
- The Quarto file link provides the code I used (in [Quarto](https://quarto.org/)) to build the slides.
- See [the resources page](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources#learning-about-quarto-and-making-the-switch-from-r-markdown) for more advice on using Quarto and transitioning to Quarto from R Markdown. 

## Announcements
 
1. I reposted the [Slides for Class 05](https://github.com/THOMASELOVE/432-classes-2023/tree/main/class05#todays-slides), fixing the typo identified in slide 20 during class, but also including new screenshots that more clearly use the `helpdat` data.
2. I added Chapters 15-28 to [the Course Notes](https://thomaselove.github.io/432-notes/).
    - I added several new data sets (used in these new chapters) to [our 432-data page](https://github.com/THOMASELOVE/432-data).
    - I added **caret** as a package to install on [our Software page](https://thomaselove.github.io/432-2023/software.html).
3. Minute Paper after Class 05 [feedback is now available](min-05-feedback.pdf).
    - Several people complained that Labs 1 and 2 were tricky. This wasn't deliberate.
    - In an effort to respond productively, I went through [the Lab 3 instructions](https://thomaselove.github.io/432-2023/lab3.html) and added minor hints.

## What Should I Be Working On?

1. [Lab 3](https://thomaselove.github.io/432-2023/lab3.html) is due Monday 2023-02-06 at 9 PM to Canvas.
2. Your [Project A Plan](https://thomaselove.github.io/432-2023/projA.html) is due Monday 2023-02-13 at 9 PM to Canvas.
3. Over the course of the term, I intend to post a few discussion questions regarding Jeff Leek's "How To Be a Modern Scientist" on our Campuswire forum. The first of these questions is now posted, and I'll keep watch on the comments through 2023-02-17 or so on that post. Please visit the forum, and weigh in on the question by reading the comments of your colleagues, and submitting your own. As incentive, more thoughtful comments will receive some bonus class participation credit.

## The Project A Plan: Key Information

In Project A, you will analyze, present and discuss two regression models, specifically a linear regression model (predicting a quantitative outcome) and a logistic regression model (predicting a binary outcome). 

- The Project A plan is the first assignment related to the Project, and is due 2023-02-13 at 9 PM to Canvas.
- We will begin discussing logistic regression in class 07, on Tuesday 2023-02-07.
- There is a [Project A Plan Quarto Template](https://raw.githubusercontent.com/THOMASELOVE/432-data/master/templates/projectAplan_template.qmd) on our [432-data page](https://github.com/THOMASELOVE/432-data) which we want you to use.
- You can either work alone, or with one other person, to complete both the Project A plan and the other parts of Project A. If you are working with a partner, exactly one of you submits everything to Canvas while the non-reporting partner submits a one-page note specifying the members of the partnership and stating that the partner will submit the work.

The [Project A plan](https://thomaselove.github.io/432-2023/projA.html#the-project-a-plan) consists of:

- a Quarto (.qmd) file containing one unnumbered, and 10 numbered sections
- an HTML result of applying the Quarto "plan" file to your data
- a copy of your (tidied) data in an .Rds file.

Key Links (all within the [Project A instructions](https://thomaselove.github.io/432-2023/projA.html))

1. Specifications related to what sort of data you need to find and [what makes a data set acceptable are found here](https://thomaselove.github.io/432-2023/projA.html#choosing-your-data).
2. A detailed description of [what you need to do in each of the Plan's sections is here](https://thomaselove.github.io/432-2023/projA.html#the-project-a-plan).
3. Again, the complete [Project A instructions are here](https://thomaselove.github.io/432-2023/projA.html).

**If you are looking for a partner for Project A** please place your name and contact information in response to the note I've posted on Campuswire, and perhaps you can connect with someone else.

## One Last Thing

From the weekly [Data is Plural newsletter](https://www.data-is-plural.com/)

**Women’s well-being.** [Camille Belmin et al.'s](https://www.nature.com/articles/s41597-022-01824-2) [LivWell dataset](https://zenodo.org/record/7277104) presents “a set of key indicators on women’s socio-economic status, health and well-being, access to basic services and demographic outcomes” in 447 regions of 52 countries from 1990 to 2019. The indicators include, for example, rates of home ownership, educational attainment, and domestic violence; they’re based primarily on [data](https://dhsprogram.com/data/) from the [Demographic and Health Surveys Program](https://dhsprogram.com/), a [USAID-funded initiative](https://dhsprogram.com/Who-We-Are/About-Us.cfm) that, since 1984, “has provided technical assistance to more than 400 surveys in over 90 countries, advancing global understanding of health and population trends in developing countries.” Read more: [An introductory Twitter thread from Belmin](https://twitter.com/BelminCamille/status/1597948618220384256).

- Note that the companion repository livwelldata allows to easily use the database in R. The R package can be downloaded following the instructions on the following git repository: https://gitlab.pik-potsdam.de/belmin/livwelldata.

## "The Play That Goes Wrong" continues through February 18

Tickets and further information are available at https://www.auroracommunitytheatre.com/. Thank you.
