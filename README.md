# List of articles about AB testing and statistics around it
## aka awesome AB testing links

## P-value
1. [Daniel Lakens wrote a great textbook on the statistical analysis. This is the link to the 1st chapter about using pvalues in hypothesis testing](https://lakens.github.io/statistical_inferences/01-pvalue.html).
2. [25 misconceptions about pvalues. Helpful resource for the interviews:)](https://pmc.ncbi.nlm.nih.gov/articles/PMC4877414/)

## Confidence interval
1. [Another link to the Daniel Lakens' textbook.](https://lakens.github.io/statistical_inferences/07-CI.html)
2. [Eppo's write up on CIs. Pay attention to the usage of the delta method for providing CIs for the % lift](https://docs.geteppo.com/statistics/confidence-intervals/statistical-nitty-gritty/)
3. [An article showing that the basic CI for the proportions can fail in certain cases. Wilson confidence interval for proportions is suggested as an alternative](https://www.econometrics.blog/post/don-t-use-the-textbook-ci-for-a-proportion/). [Part 2 is here](https://www.econometrics.blog/post/the-wilson-confidence-interval-for-a-proportion/)

## MDE
1. [Eppo's article about MDE. Great resource for building intuition around the concept](https://docs.geteppo.com/statistics/sample-size-calculator/mde/)
2. [Penn State Eberly College of science STAT415 online textbook with a simple example of the MDE formula derivation](https://online.stat.psu.edu/stat415/lesson/25/25.3)
3. [Apple's article with an extensive list of formulas for MDE with](https://arxiv.org/abs/2305.16459)
4. [Ozon's (huge russian online marketplace) article about AB testing with an advanced case of the MDE formula (multiple groups and multiple comparisons correction)](https://habr.com/ru/companies/ozontech/articles/712306/)
5. [Booking's sample size calculator. Not only conversion metrics are included(!)](https://bookingcom.github.io/powercalculator/)
6. [Kirill Kochnev's article discussing the consequences of unequal sample sizes on power of an AB test (e.g. what will happen to power if you split your auditory as 30/70 instead of 50/50)\[RU\]](https://koch-kir.medium.com/мощность-а-в-теста-с-неравными-выборками-4859ce2ddb13)

## CUPED
1. [Original paper](https://www.researchgate.net/publication/237838291_Improving_the_Sensitivity_of_Online_Controlled_Experiments_by_Utilizing_Pre-Experiment_Data)
2. [Detailed review of CUPED from Matteo Courthoud. Code and references to the FWL theorem inside. Highly recommended.](https://matteocourthoud.github.io/post/cuped/)
3. [Cool blog post with examples beyond CUPED. The author tries to fit a random forest on the pre experiment data and touches upon the issue of overfitting](http://www.degeneratestate.org/posts/2018/Jan/04/reducing-the-variance-of-ab-test-using-prior-information/)
4. [Eppo's documentation about CUPED](https://docs.geteppo.com/statistics/cuped/)
5. [Guide to the sample size estimation when using CUPED. TLDR: estimate rho on the historical data](https://www.statsig.com/blog/how-to-plan-test-duration-cuped)
6. [One the best lectures about the mechanics of CUPED in russian \[RU\]. Lots of Kudos to Philipp for uploading his HSE lectures to YouTube](https://www.youtube.com/watch?v=nGNeehLcXm0&list=PLNKXA-74YGLiK5Ig_evBlT8PqkQMexFIv&index=14)

## Ratio metrics
1. [The article by Alex Deng with the introduction of the delta method for the ratio metrics](https://alexdeng.github.io/public/files/kdd2018-dm.pdf)
2. [The Rice university handout about delta method from the Alex Papanicolaou](https://www.stat.rice.edu/~dobelman/notes_papers/math/TaylorAppDeltaMethod.pdf)
3. [Linearization article. One of the most well known and well performing alternatives to the delta method](https://www.researchgate.net/publication/322969314_Consistent_Transformation_of_Ratio_Metrics_for_Efficient_Online_Controlled_Experiments)
4. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/740476/)

## Multiple testing problem
1. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/842426/)

## Bootstrap
1. [One the best lectures about bootstrap in russian \[RU\]. Lots of Kudos to Philipp for uploading his HSE lectures to YouTube](https://www.youtube.com/watch?v=CjVNOeX-Ahk&list=PLNKXA-74YGLjDOtDSZEFoy1yP-3AfiHUC&index=20)
2. [X5 Retail article with code and simulations \[RU\]](https://habr.com/ru/companies/X5Tech/articles/679842/)
3. [Google introduces Poisson bootstrap in 2015:)](https://www.unofficialgoogledatascience.com/2015/08/an-introduction-to-poisson-bootstrap26.html)

## MISC
1. [Must read article with simulations for different statistical criteria. IMHO: the code for the simulations is as interesting as the rest of the article](https://vkteam.medium.com/practitioners-guide-to-statistical-tests-ed2d580ef04f)
2. [Very cool textbook by Michael Clark. All the most popular statistical models coded from scratch in R and sometimes in Python](https://m-clark.github.io/models-by-example/zi.html)
3. [Friendly Econometrics textbook \[RU\]. One of the best introductions to the linear regression, that I have seen.](https://books.econ.msu.ru/Introduction-to-Econometrics/)
