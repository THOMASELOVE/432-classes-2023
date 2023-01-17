# 432 Class 01: 2023-01-17

[Main Website](https://thomaselove.github.io/432-2023/) | [Calendar](https://thomaselove.github.io/432-2023/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2023/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | PDF | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
01 | 2023-01-17 | **[Slides 01](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides01.pdf)** | **[Code 01](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides01.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

- The PDF link provides the version of the slides that I suggest you focus on during class.
- The Quarto file link provides the code I used (in [Quarto](https://quarto.org/)) to build the slides.
- We attempt to record every 432 class and post the recording to Canvas.

## Announcements
 
1. Welcome to 432! Please complete the Welcome to 432 Survey at <https://bit.ly/432-2023-welcome-survey> by noon tomorrow. Thanks so much to those of you who've done this already.
2. You can do this. It's a lot of work, but it's worth it.

## References from Today's Slides

- Course Mechanics
    - [Main Website](https://thomaselove.github.io/432-2023/), [Calendar](https://thomaselove.github.io/432-2023/calendar.html), [Syllabus](https://thomaselove.github.io/432-syllabus-2023/), [Course Notes](https://thomaselove.github.io/432-notes/)
    - [Software](https://thomaselove.github.io/432-2023/software.html) ([Updating/Installing R & RStudio](https://thomaselove.github.io/432-2023/software.html#installing-r-and-rstudio), necessary [R Packages](https://thomaselove.github.io/432-2023/software.html#r-packages-to-install))
    - Get Data (and Code, Quarto templates) at our [432-data page](https://github.com/THOMASELOVE/432-data)
    - Assignments (including instructions for [all 8 Labs](https://thomaselove.github.io/432-2023/lab1.html), [2 Projects](https://thomaselove.github.io/432-2023/projA.html)) plus [2 Quizzes](https://thomaselove.github.io/432-2023/quiz1.html), deadlines in [Calendar](https://thomaselove.github.io/432-2023/calendar.html)
    - [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources) (books, articles, videos, etc.)
    - Key Links (including [Canvas](https://canvas.case.edu/), [Campuswire](https://campuswire.com/), [Shared Drive](https://docs.google.com/document/d/1A6-P4TRXrCZVAqfDWw_s75lBGID9wHiaJjbsjltXojs/edit?usp=sharing) and [Minute Papers](https://github.com/THOMASELOVE/432-minute-2023))
    - [Contact Us](https://thomaselove.github.io/432-2023/contact.html) (Campuswire + TA office hours and `Thomas` dot `Love` at `case` dot `edu`)
- Why I Write Dates the Way I Do
    - [XKCD: Public Service Announcement](https://xkcd.com/1179/)
    - Some more [from Wikipedia on ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
- Data Organization in Spreadsheets, 
    - Karl W. Broman & Kara H. Woo (2018) [Data Organization in Spreadsheets]([pdf/Broman_and_Woo_2018_Data_Organization_in_Spreadsheets.pdf](https://github.com/THOMASELOVE/432-classes-2023/blob/main/sources/pdf/Broman_and_Woo_2018_Data_Organization_in_Spreadsheets.pdf)), *The American Statistician*, 72:1, 2-10, DOI: [10.1080/00031305.2017.1375989](https://doi.org/10.1080/00031305.2017.1375989)
    - [Tidy Data by Hadley Wickham](https://www.jstatsoft.org/article/view/v059i10) in *J of Statistical Software*
    - [R for Data Science, 2nd edition](https://r4ds.hadley.nz/) or [1st edition](https://r4ds.had.co.nz/)
    - [How to Share Data with a Statistician](https://github.com/jtleek/datasharing) by Jeff Leek
    - Shannon Ellis and Jeff Leek [How to Share Data for Collaboration (pdf)](https://peerj.com/preprints/3139v5.pdf)
- Naming Things and Getting Organized
    - [XKCD: Documents](https://xkcd.com/1459/)
    - Jenny Bryan's slides on [Naming Things (pdf)](http://www2.stat.duke.edu/~rcs46/lectures_2015/01-markdown-git/slides/naming-slides/naming-slides.pdf), or at [Slideshare](https://www.slideshare.net/milkers/naming-things), or at [SpeakerDeck](https://speakerdeck.com/jennybc/how-to-name-files)
    - Jenny's [Golden Rule of Naming Files and Other Things tweet](https://twitter.com/jennybryan/status/807805087544328192?lang=en)
    - [Project-oriented workflow](https://www.tidyverse.org/blog/2017/12/workflow-vs-script/) from Jenny Bryan
    - The "Version Control" cartoon comes from [Geek and Poke](https://geek-and-poke.com/)
    - [Good Enough Practices in Scientific Computing](http://bit.ly/good-enuff)
- Switching from R Markdown to Quarto
    - I've gathered resources for helping with this transition [on our Sources page](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources#learning-about-quarto-and-making-the-switch-from-r-markdown).
    - Virtually any code you have written in R Markdown can be run using Quarto instead, by simply switching the file extension from .Rmd to .qmd.
    - It's still worth it to learn about how Quarto works, and why it differs from R Markdown when it does.
- Building and Validating Linear Prediction Models
    - See the [431 Course Notes](https://thomaselove.github.io/431-notes/), as well as the [432 Course Notes](https://thomaselove.github.io/432-notes/). Both will remain online until 2023-06-01.

## TA Office Hours

TA Office Hours (delivered via Zoom) begin **Friday 2023-01-20**, and run through Sunday 2023-04-30, other than Spring Break (no office hours March 10-17.) We have office hours scheduled every day of the week.

- The schedule is now available on [the Calendar](https://thomaselove.github.io/432-2023/calendar.html) and [the Contact Us page](https://thomaselove.github.io/432-2023/contact.html). 
- Details on joining the Zoom sessions for Office Hours will be posted to our Shared (Google) Drive on Thursday 2023-01-19.
- No appointment is necessary - please just drop in.

Our [Campuswire discussion forum](https://thomaselove.github.io/432-2023/contact.html#once-class-starts) is open 24 hours a day, 7 days a week, and is a great place to ask (and answer) questions.

## What Should I Be Working On?

By Wednesday 2023-01-18 at Noon:

1. Get officially registered (SIS) for the right flavor of the course (PQHS 432, CRSP 432 or MPHP 432) if you're not already.
2. Welcome to 432 survey at https://bit.ly/432-2023-welcome-survey complete by noon tomorrow. 
    - Thanks to the 29 of you who've already done this as of 9:40 this morning.
3. Accept your invitation to Campuswire (see your email or [visit here](https://thomaselove.github.io/432-2023/contact.html#once-class-starts)) and then answer my little poll question there, please.

Before our next class Thursday 2023-01-19 at 1 PM

1. Review the [website](https://thomaselove.github.io/432-2023/) and [Calendar](https://thomaselove.github.io/432-2023/calendar.html), and skim the [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) and [Course Notes](https://thomaselove.github.io/432-notes/).
2. Buy Jeff Leek's How to be a Modern Scientist (then read this by the end of January - it should take ~ 4 hours.)
3. Get started installing or updating your R and RStudio and install these R Packages and data/code from 432-Data.
4. Get started on [Lab 1](https://thomaselove.github.io/432-2023/lab1.html), which is due Monday 2023-01-23 at 9 PM. The "431 Review" Chapters from the [432 Course Notes](https://thomaselove.github.io/432-notes/) should be helpful.

## One Last Thing

I am in a play that runs on Friday and Saturday evenings at 8 PM starting January 27 and running through February 18 at [Aurora Community Theatre](https://www.auroracommunitytheatre.com/), in Aurora, Ohio. I'm always delighted to see anyone I know at any show I do. Please do come if you are interested, and if you are comfortable being around people who are unmasked. 

It's called "[The Play That Goes Wrong](https://www.youtube.com/watch?v=DOWO4gq-whg)." It is widely regarded as one of the funniest plays ever produced, and is sometimes referred to as a hybrid of Monty Python and Sherlock Holmes. I am playing a leading role, that of Chris, the play's director and one of its stars, and I'm not going to tell you anything more about it, except that I am exceedingly proud of the show, and think you will like it. 

If you'd like to come, that would be great, and all of the information you need to buy tickets (they are **selling very quickly**) is available by clicking the "Buy Tickets" link at <https://www.auroracommunitytheatre.com/>. Tickets are $20, and $16 for those ages 18 and under. The theater is about a 40-45 minute drive from the CWRU campus, east and south of Cleveland.

If you wouldn't like to come, that's **100% OK**. I have various professional roles (as a teacher, for example) where I have some nominal control over other people's happiness or work. If you're someone who interacts with me professionally, please feel no obligation to attend a show I'm in. Attending (or not attending) a show I'm in carries no weight with me at all in any professional capacity.

