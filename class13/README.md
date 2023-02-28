# 432 Class 13: 2023-02-28

[Main Website](https://thomaselove.github.io/432-2023/) | [Calendar](https://thomaselove.github.io/432-2023/calendar.html) | [Syllabus](https://thomaselove.github.io/432-syllabus-2023/) | [Notes](https://thomaselove.github.io/432-notes/) | [Contact Us](https://thomaselove.github.io/432-2023/contact.html) | [Canvas](https://canvas.case.edu) | [Data and Code](https://github.com/THOMASELOVE/432-data) | [Sources](https://github.com/THOMASELOVE/432-classes-2023/tree/main/sources)
:-----------: | :--------------: | :----------: | :---------: | :-------------: | :-----------: | :------------: |:------:
for everything | for deadlines | expectations | from Dr. Love | ways to get help | lab submission | for downloads | to read

## Today's Slides

Class | Date | PDF | Quarto .qmd | Recording
:---: | :--------: | :------: | :------: | :-------------:
13 | 2023-02-28 | **[Slides 13](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides13.pdf)** | **[Code 13](https://github.com/THOMASELOVE/432-slides-2023/blob/main/slides13.qmd)** | Visit [Canvas](https://canvas.case.edu/), select **Zoom** and **Cloud Recordings**

## Supplemental Materials / Sources for Today

Today we'll focus on:

1. thinking about power issues through retrospective design
2. robust linear models using Huber weights, or bisquare weights or quantile regression.

- Andrew Gelman and John Carlin [Beyond Power Calculations: Assessing Type S (Sign) and Type M (Magnitude) Errors](references/Gelman_Carlin_2014_Beyond_Power_Calculations.pdf)
- Ronald L. Wasserstein, Allen L. Schirm & Nicole A. Lazar (2019) [Moving to a World Beyond "p < 0.05"](https://www.tandfonline.com/doi/full/10.1080/00031305.2019.1583913), *The American Statistician*, 73: sup1, 1-19, DOI: [10.1080/00031305.2019.1583913](https://doi.org/10.1080/00031305.2019.1583913). [PDF available here, too](references/ASA_2019_A_World_Beyond.pdf).
- Ronald L. Wasserstein & Nicole A. Lazar (2016) [The ASA's Statement on p-Values: Context, Process, and Purpose](https://www.tandfonline.com/doi/full/10.1080/00031305.2016.1154108), *The American Statistician*, 70:2, 129-133, DOI:
[10.1080/00031305.2016.1154108](https://doi.org/10.1080/00031305.2016.1154108). [PDF available here, too](references/ASA_2016_Pvalues_Context_Process_Purpose.pdf).
- Jeff Leek and Roger Peng's article in Nature (2015) [P values are just the tip of the iceberg](references/Leek_and_Peng_2015_Pvalues_Nature.pdf)
- https://stats.oarc.ucla.edu/r/dae/robust-regression/ provides a relevant example, which I drew on in building today's slides about the crimestat data.
- Some theoretical discussion of the motivation behind various robust regression procedures can be found in [Robust Regression](https://socialsciences.mcmaster.ca/jfox/Books/Companion/appendices/Appendix-Robust-Regression.pdf) by John Fox and Sanford Weisberg.

### Need to have a tough talk with someone about statistical significance, and/or p values?

- The ASA Section on Teaching of Statistics in the Health Sciences has [some interesting material](https://tshsblog.wixsite.com/main/single-post/2018/05/08/ReadyResources-Publications-for-teaching-p-values)
- I've given these posts: [Why I've lost faith in p values, part 1](https://lucklab.ucdavis.edu/blog/2018/4/19/why-i-lost-faith-in-p-values) and [Why I've lost faith in p values, part 2](https://lucklab.ucdavis.edu/blog/2018/4/28/why-ive-lost-faith-in-p-values-part-2) to a few people. Maybe they'll help you.
- "[Abandoning statistical significance is both sensible and practical](https://peerj.com/preprints/27657/)" by Amrhein, Gelman, Greenland and McShane at PeerJ Preprints.
- Frank Harrell's post about "[Language for communicating frequentist results about treatment effects](https://discourse.datamethods.org/t/language-for-communicating-frequentist-results-about-treatment-effects/934)"
- "[Calculating Observed Power Is Just Transforming Noise](https://lesslikely.com/statistics/observed-power-magic/) at [LessLikely](https://lesslikely.com/)
    - "A discussion of events that transpired in the past year, where a group of surgical researchers decided to ignore much of the statistical literature and promote a highly misleading practice of calculating post-hoc power using the observed effect size."
    - Some related pieces at LessLikely include "[Misplaced Confidence in Observed Power](https://lesslikely.com/statistics/misplaced-power/)" and "[P-Values Are Tough and S-Values Can Help](https://lesslikely.com/statistics/s-values/)".
- Andrew Gelman: [Statistical-significance thinking is not just a bad way to publish, it’s also a bad way to think](https://statmodeling.stat.columbia.edu/2019/03/16/statistical-significance-thinking-is-not-just-a-bad-way-to-publish-its-also-a-bad-way-to-think/) - the money quote: "it’s ultimately not about what it takes, or should take, to get a result published, but rather how we as researchers can navigate through uncertainty and not get faked out by noise in our own data."
