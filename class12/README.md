# 432 Class 12: 2023-02-23

[Main Website](https://thomaselove.github.io/432-2023/) | [Calendar](https://thomaselove.github.io/432-2023/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2023/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | PDF | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
12 | 2023-02-23 | **[Slides 12](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides12.pdf)** | **[Code 12](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides12.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

![](https://imgs.xkcd.com/comics/data_quality.png) [Link to XKCD](https://xkcd.com/2739)

## Announcements

1. Feedback from Dr. Love on all Project A Plans should be posted to Canvas **by class time**. Those of you who need to do a third version need to get that in by Saturday at 9 AM (that's 9 in the morning, not evening.)
    - The status report remains [at this link](https://github.com/THOMASELOVE/432-classes-2023/blob/main/projectA/plans.md). I have some more comments below.
2. Feedback on the Minute Paper after Class 11 [is now available](min-11-feedback.pdf).
3. [Quiz 1 materials](https://thomaselove.github.io/432-2023/quiz1.html) will be available **by 5 PM today**. 
    - [Quiz 1](https://thomaselove.github.io/432-2023/quiz1.html) is due on Monday 2023-02-27 at 9 PM. All of your responses must be on the Google Form by that time.
    - Read the instructions carefully before starting the Quiz.
    - To ask questions about the Quiz, either post them as questions (to the instructors and TAs only) on Campuswire, or email `431-help at case dot edu`. TAs will not answer questions about the Quiz during their office hours this weekend.

## Some Project A Plan Comments I want to ensure everyone sees

Here are a few Project A Plan comments I listed repeatedly in my comments on Canvas, but might have missed in your case. Please read and heed these, if they apply to your situation, regardless of whether I caught the issue in your case.

1. Avoid using `::` when you don't have to. For example, you don't need Hmisc::describe(), just describe() if you've properly loaded Hmisc (or rms, which automatically loads Hmisc.) Same goes for virtually every other place where you might find `::` - the notable exceptions are `knitr::opts_chunk$set` at the start of your R Packages and Setup section, and `xfun::session_info()` in your Session Information.
2. Within section 3, you need to filter to complete cases on your linear regression outcome and your logistic regression outcome (but not on anything else) so that your resulting tibble has complete data on those two variables. Making these changes will, of course, alter your sections 4-7 as well. If you have a large data set from which you're sampling, I encourage you to do this filtering before selecting your random sample. 
3. If you have a binary variable in your work that is coded 1 = Yes and 2 = No, you need to change that to 1 = Yes and 0 = No (or to a factor with values Yes and No) in section 3 of the project.
4. Also, if you're working alone, it's OK to use either "I" or "we" to refer to yourself (i.e. we cleaned the data...) in your project work, but if you're working with a partner, it must be "We".
5. Specify in Section 2 (The Subjects) the number of subjects you will eventually have in your tidied tibble (and thus in your linear and logistic analyses.)
6. If your research question is not in the form "How effectively can we predict [your outcome] using [your predictors]?" you should consider whether changing to that would be a more accurate reflection of what your analyses will actually be doing. In almost every case, it would.
7. Don't include subsections that you're not using. Be sure you have a good reason for not using any of our suggested subsections.

## Materials for the `bradley` example

- The original source is Steven M. Bradley, Joleen A. Borgerding, G. Blake Wood, et al. [Incidence, Risk Factors, and Outcomes Associated With In-Hospital Acute Myocardial Infarction](https://jamanetwork.com/journals/jamanetworkopen/fullarticle/2720923) *JAMA Netw Open* 2019; 2(1): e187348. doi:10.1001/jamanetworkopen.2018.7348.
- [JAMA Table Creation Instructions](https://jama.jamanetwork.com/data/ifora-forms/jama/tablecreationinst.pdf) (pdf)
- The bradley_sim file: [.qmd code](https://github.com/THOMASELOVE/432-slides-2023/blob/main/c12/bradley_sim.qmd), [.html result at RPubs](https://rpubs.com/TELOVE/bradley-simulate-432)
- The bradley_table1 file: [.qmd code](https://github.com/THOMASELOVE/432-slides-2023/blob/main/c12/bradley_table1.qmd), [.html result at RPubs](https://rpubs.com/TELOVE/bradley-table1-432)
- The [bradley.csv](https://github.com/THOMASELOVE/432-slides-2023/blob/main/c12/data/bradley.csv) data file
- The [bradley_table1_result.csv](https://github.com/THOMASELOVE/432-slides-2023/blob/main/c12/data/bradley_table1_result.csv) file

[Chapter 18 in the Course Notes](https://thomaselove.github.io/432-notes/) covers the topic of building a Table 1 far more extensively, with two detailed examples. Those notes should be helpful for doing the Table 1 work required in [Lab 5](https://thomaselove.github.io/432-2023/lab5.html).

## One Last Thing


