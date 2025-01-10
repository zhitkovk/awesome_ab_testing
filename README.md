# List of articles on A/B testing and related statistical concepts
## aka awesome AB testing links grouped by the topic

## Basics
### P-value
1. [Daniel Lakens wrote a great textbook on the statistical analysis. This is the link to the 1st chapter about using pvalues in hypothesis testing](https://lakens.github.io/statistical_inferences/01-pvalue.html).
2. [25 misconceptions about pvalues. Helpful resource for the interviews:)](https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/)

### Confidence intervals
1. [Another link to the Daniel Lakens' textbook.](https://lakens.github.io/statistical_inferences/07-CI.html)
2. [Eppo's write up on CIs. Pay attention to the usage of the delta method for providing CIs for the % lift](https://docs.geteppo.com/statistics/confidence-intervals/statistical-nitty-gritty/)
3. [An article showing that the basic CI for the proportions can fail in certain cases. Wilson confidence interval for proportions is suggested as an alternative](https://www.econometrics.blog/post/don-t-use-the-textbook-ci-for-a-proportion/). [Part 2 is here](https://www.econometrics.blog/post/the-wilson-confidence-interval-for-a-proportion/)

### MDE
1. [Eppo's article about MDE. Great resource for building intuition around the concept](https://docs.geteppo.com/statistics/sample-size-calculator/mde/)
2. [Penn State Eberly College of science STAT415 online textbook with a simple example of the MDE formula derivation](https://online.stat.psu.edu/stat415/lesson/25/25.3)
3. [Apple's article with an extensive list of MDE formulas for different scenarios (e.g. how to estimate MDE in case of ratio metric)](https://arxiv.org/abs/2305.16459)
4. [Ozon's article about AB testing with an advanced case of the MDE formula (multiple groups and multiple comparisons correction) \[RU\]](https://habr.com/ru/companies/ozontech/articles/712306/)
5. [Booking's sample size calculator. Not only conversion metrics are included(!)](https://bookingcom.github.io/powercalculator/)
6. [Kirill Kochnev's article discussing the consequences of unequal sample sizes on power of an AB test (e.g. what will happen to power if you split your auditory as 30/70 instead of 50/50)\[RU\]](https://koch-kir.medium.com/мощность-а-в-теста-с-неравными-выборками-4859ce2ddb13)

### Sample Ratio Mismatch
1. [A fundamental article about SRM with multiple examples of the SRM origin and ways to detect it](https://www.researchgate.net/publication/334720020_Diagnosing_Sample_Ratio_Mismatch_in_Online_Controlled_Experiments_A_Taxonomy_and_Rules_of_Thumb_for_Practitioners)

### Multiple testing problem
1. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/842426/)

## Specific statistical technics

### CUPED
1. [Original paper](https://www.researchgate.net/publication/237838291_Improving_the_Sensitivity_of_Online_Controlled_Experiments_by_Utilizing_Pre-Experiment_Data)
2. [Detailed review of CUPED from Matteo Courthoud. Code and references to the FWL theorem inside. Highly recommended.](https://matteocourthoud.github.io/post/cuped/)
3. [Cool blog post with examples beyond CUPED. The author tries to fit a random forest on the pre experiment data and touches upon the issue of overfitting](http://www.degeneratestate.org/posts/2018/Jan/04/reducing-the-variance-of-ab-test-using-prior-information/)
4. [Eppo's documentation about CUPED](https://docs.geteppo.com/statistics/cuped/)
5. [Guide to the sample size estimation when using CUPED. TLDR: estimate rho on the historical data](https://www.statsig.com/blog/how-to-plan-test-duration-cuped)
6. [One the best lectures about the mechanics of CUPED in Russian \[RU\]. Lots of Kudos to Philipp for uploading his HSE lectures to YouTube](https://www.youtube.com/watch?v=nGNeehLcXm0&list=PLNKXA-74YGLiK5Ig_evBlT8PqkQMexFIv&index=14)

### Bootstrap
1. [One of the best lectures about bootstrap in Russian \[RU\]. Kudos to Philipp for sharing his HSE lectures on YouTube](https://www.youtube.com/watch?v=CjVNOeX-Ahk&list=PLNKXA-74YGLjDOtDSZEFoy1yP-3AfiHUC&index=20)
2. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/679842/)
3. [Google introduces Poisson bootstrap in 2015:)](https://www.unofficialgoogledatascience.com/2015/08/an-introduction-to-poisson-bootstrap26.html)

### Ratio metrics
1. [The article by Alex Deng with the introduction of the delta method for the ratio metrics](https://alexdeng.github.io/public/files/kdd2018-dm.pdf)
2. [The Rice university handout about delta method from the Alex Papanicolaou](https://www.stat.rice.edu/~dobelman/notes_papers/math/TaylorAppDeltaMethod.pdf)
3. [Linearization article. One of the most well known and well performing alternatives to the delta method](https://www.researchgate.net/publication/322969314_Consistent_Transformation_of_Ratio_Metrics_for_Efficient_Online_Controlled_Experiments)
4. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/740476/)

### Team draft interleaving (TDI)
1. [Must read: "Large-Scale Validation and Analysis of Interleaved Search Evaluation"](https://www.cs.cornell.edu/people/tj/publications/chapelle_etal_12a.pdf)
2. [Netflix's article with the study of the TDI and classic AB test codirectionality](https://netflixtechblog.com/interleaving-in-online-experiments-at-netflix-a04ee392ec55?gi=bd185003adcf)
3. [Erik Bernhardson on interleaving, with examples of both balanced and team-draft methods](https://www.youtube.com/watch?v=-1npOZBQ7AQ)
4. [Roman Poborchy's AIC meetup presentation with great slides and easy to follow examples \[RU\]](https://www.youtube.com/watch?v=voY7waRb_D0)

### Switchback experiments (to be added)
1. [Doordash's introductory article with the simulations](https://careersatdoordash.com/blog/experiment-rigor-for-switchback-experiment-analysis/)

### Sequential testing (to be added)
1. TODO

## MISC
1. [Must read article with simulations for different statistical criteria. IMHO: the code for the simulations is as interesting as the rest of the article](https://vkteam.medium.com/practitioners-guide-to-statistical-tests-ed2d580ef04f)
2. [Very cool textbook by Michael Clark. All the most popular statistical models coded from scratch in R and sometimes in Python. E.g. you can check the maximum likelihood code for the logistic regression](https://m-clark.github.io/models-by-example/zi.html)
3. [Friendly Econometrics textbook \[RU\]. One of the best introductions to the linear regression, that I have seen.](https://books.econ.msu.ru/Introduction-to-Econometrics/)
