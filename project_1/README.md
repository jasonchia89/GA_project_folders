# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) 

# Project 1: 2017-2018 SAT and ACT analysis

### Context and Problem Statement

Most american colleges and universities take into account the scores of 2 main entrance exams - Scholastic Aptitude Test (SAT) and American College Test (ACT) - when assessing students' eligibility for college placement. The SAT is administered by the College Board while the ACT is administered by the ACT organisation and both are non-profit organizations that seek to expand college access for all students. Most states either go for SATs or ACTs, seldom both. There has been a surge in popularity for ACT relative to SAT in recent years and this has resulted in a heightened sense of competition between the College Board and ACT in capturing as many states as possible for college entrance exam administration.

The new format for the SAT was released in March 2016, and relative to the ACT which tests students mostly on highly mathematical concepts such as trigonometry and geometry for its Math component, the SAT Math sub-test includes more applied concepts such as qualitative and quantitative data analysis which would be more useful beyond college education, when students graduate and enter the workforce. It is thus important to enhance SAT participation, especially in state(s) that has/ve poor participation rates and 
considerable high school graduate population size that has yet to take the SAT.

--- 

[Executive Summary](#ExecutiveSummary)

[Interpretation of Results](#Interpretation-of-results)

[Business Recommendations](#Business-recommendations)

[Sources](#Sources)

### Executive Summary

Datasets containing scores, sub-test scores, and participation rates for SAT and ACT in 2017 and 2018 were used for this analysis. The data was cleaned and combined into one master dataset for exploratory analysis. The data dictionary below illustrates the variables available for analysis. 

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|ACT 2017, ACT 2018, SAT 2017, SAT 2018|Name of each US state (51 altogether as District of Columbia was included in addition to Washington)| 
|**act_2017_participation**|*int*|ACT 2017|ACT 2017 Participation Rate in each US state|
|**act_2017_english**|*float*|ACT 2017|Mean scaled score (min 1, max 36) for the English test component in ACT 2017 by each US state|
|**act_2017_math**|*float*|ACT 2017|Mean scaled score (min 1, max 36) for the Math test component in ACT 2017 by each US state|
|**act_2017_reading**|*float*|ACT 2017|Mean scaled score (min 1, max 36) for the Reading test component in ACT 2017 by each US state|
|**act_2017_science**|*float*|ACT 2017|Mean scaled score (min 1, max 36) for the Science test component in ACT 2017 by each US state|
|**act_2017_composite**|*float*|ACT 2017|Average of mean scaled scores (min 1, max 36) from English, Math, Reading and Science test components in ACT 2017 by each US state|
|**sat_2017_participation**|*int*|SAT 2017|SAT 2017 Participation Rate in each US state|
|**sat_2017_erw**|*int*|SAT 2017|Mean score (min 200, max 800) for the Evidence-Based Reading and Writing Section component of SAT 2017 by each US state|
|**sat_2017_math**|*int*|SAT 2017|Mean score (min 200, max 800) for the Math Section component of SAT 2017 by each US state|
|**sat_2017_total**|*int*|SAT 2017|Sum of mean scores (min 400, max 1600) from both Evidence-Based Reading and Writing and Math Section components of SAT 2017 by each US state|
|**act_2018_participation**|*int*|ACT 2018|ACT 2018 Participation Rate in each US state|
|**act_2018_english**|*float*|ACT 2018|Mean scaled score (min 1, max 36) for the English test component in ACT 2018|
|**act_2018_math**|*float*|ACT 2018|Mean scaled score (min 1, max 36) for the Math test component in ACT 2018|
|**act_2018_reading**|*float*|ACT 2018|Mean scaled score (min 1, max 36) for the Reading test component in ACT 2018|
|**act_2018_science**|*float*|ACT 2018|Mean scaled score (min 1, max 36) for the Science test component in ACT 2018|
|**act_2018_composite**|*float*|ACT 2018|Average of mean scaled scores (min 1, max 36) from English, Math, Reading and Science test components in ACT 2018|
|**sat_2018_participation**|*int*|SAT 2018|SAT 2018 Participation Rate in each US state|
|**sat_2018_erw**|*int*|SAT 2018|Mean score (min 200, max 800) for the Evidence-Based Reading and Writing Section component of SAT 2018 by each US state|
|**sat_2018_math**|*int*|SAT 2018|Mean score (min 200, max 800) for the Math Section component of SAT 2018 by each US state|
|**sat_2018_total**|*int*|SAT 2018|Sum of mean scores (min 400, max 1600) from both Evidence-Based Reading and Writing and Math Section components of SAT 2018 by each US state|

Iowa was chosen as the state to focus the College Board's efforts on when seeking to boost SAT participation rate due to its vast population of high school students that have yet to take SATs and that it would be easier to win it over given that it is a state that has yet to stipulate an ACT requirement for high school graduation or college entrance. Strategies pertaining to awareness campaigns and initiatives catered for the convenience of students to take the SATs are some recommendations to boost SAT participation rates.

### Interpretation of Results
Initial analyses revealed marginal inverse relationships between SAT total scores and SAT participation rates as well as between SAT and ACT participation rates that when coupled with outside research suggests that it would be most effective to target states that are SAT/ACT agnostic to boost SAT participation rates. Iowa was targeted as it has shown to neither adopt SAT nor ACT as a college entrance requirement, and thus constitutes a state with potential to take up SAT testing and expand its students' college access. It was also ranked one of the bottom 3 states in terms of SAT'17 participation rates based on numerical summaries derived from the master dataset. Its SAT'17 and SAT'18 participation rates were as low as 2% and 3% respectively.

However, it is recognized that more information is needed to do a more comprehensive statistical analysis of SAT and ACT participation rates in the US given that only scores and participation rates were provided. Based on online resources, potentially crucial and relevant factors such as highest parental education levels, income/wealth/poverty status of families, and even demographics such as race/ethnicity could have an impact on SAT participation rates that could be analyzed to discover hidden insights and potential strategies that may be more effective in enhancing SAT participation rates or identifying more accurately, the states that the College Board should target its efforts to maximize SAT participation.

### Business Recommendations

Given that the implementation of a SAT School Day programme where free SAT exams are offered to graduating high school students on a regular school day has helped boost SAT participation rates in other states like Florida in the past, such a recommendation could be considered in Iowa too, especially when it is not entrenched in administering ACTs yet. It would be more unlikely for Iowa to take up SAT if it has already begun administering ACT since either SAT or ACT is sufficient as a means of college-readiness assessment for most colleges and administering both for each graduating high school student could be unduly taxing for them and redundant. Furthermore, Iowa has a considerable number of high school graduates in 2017 that have yet to take the SAT and they represent substantial real estate for SAT administration. 

### Sources
https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/
https://www.act.org/content/dam/act/unsecured/documents/cccr2017/ACT_2017-Average_Scores_by_State.pdf
https://www.testive.com/colorado-sat-change-2017/
https://www.collegeraptor.com/getting-in/articles/act-sat/preference-act-sat-state-infographic/
https://www.hanoverresearch.com/media/Best-Practices-to-Increase-SAT-Participation-1.pdf
https://www.princetonreview.com/college-advice/act-math-practice
https://www.kaptest.com/study/sat/whats-tested-on-the-sat-math-section/
https://reports.collegeboard.org/pdf/2018-district-columbia-sat-suite-assessments-annual-report.pdf
https://www.edweek.org/ew/section/multimedia/states-require-students-take-sat-or-act.html
https://magoosh.com/hs/act/2017/states-that-require-the-act-or-sat/
https://www.orlandosentinel.com/news/education/os-ne-sat-scores-florida-20190924-2ycpuogc2ndkrkwzdrkrjgrg64-story.html