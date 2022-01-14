Welcome to DSCI 562: Regression II
============================

Let us explore regression techniques beyond Ordinary Least-Squares! What if the response is still continuous but non-negative, or our observations are not independent anymore? Maybe the response is binary, a count, or categorical. Moreover, what if we have censored data? In many other cases, we might not be interested in modelling the conditioned mean response. Different Data Science projects will require making inference on different conditioned response quantiles. This course covers useful extensions to ordinary linear regression: generalized linear models, mixed-effects, smoothing, quantile and robust regression, and techniques for dealing with missing data.

**Slack Channel**: [Access here.](https://ubc-mds.slack.com/messages/562_regr-2)

## Course Learning Objectives

By the end of the course, students are expected to:

- Describe the value of making parametric assumptions in regression.
- Fit model functions that represent probabilistic quantities besides the mean.
- Identify situations where ordinary linear regression is sub-optimal, and apply alternative regression methods that better address the situation.

## Teaching Team

| Position | Name | Slack Handle | GHE Handle  |
| :---:    | :---:| :---:        | :---:       |
|  Lecture/Lab Instructor | [Alexi Rodríguez-Arelis](https://alexrod.netlify.app) | `@Alexi` | `@alexrod6`   |
| Teaching Assistant | Yulia Egorova | `@Yulia Egorova ` | `@yulia90` |
| Teaching Assistant | Katie Florko | `@Katie Florko` | `@kflork` |
| Teaching Assistant | Siddhesh Khandelwal | `@Siddhesh` | `@skhandel` |
| Teaching Assistant | Mohamad Amin Mohamadi | `@Amin` | `@lemohama` |
| Teaching Assistant | Alireza Naderi  | `@Alireza Naderi` | `@alinad01` |
| Teaching Assistant | Shuyi Tan  | `@Shuyi Tan` | `@shuyitan` |

## Lecture Schedule

This course occurs during **Block 4** in the 2021/22 school year.

| Lecture | Topic | Suggested Reading Material |
| :---:   | --- | --- |
| 1 | Beyond Ordinary Least-Squares! | <ul><li>Chapter 1 (Review of Multiple Linear Regression): [BMLR](https://bookdown.org/roback/bookdown-BeyondMLR/ch-MLRreview.html) <li> Logarithmic Transformations in Regression: [Do You Transform Back Correctly?](https://libkey.io/libraries/498/articles/62044506/full-text-file?utm_source=api_542) </ul> |
| 2 | Foundations of Generalized Linear Models: Binary Logistic and Count Regressions | <ul><li>Basics of GLMs: [BMLR](https://bookdown.org/roback/bookdown-BeyondMLR/ch-glms.html) 5.3 <li>Binomial logistic regression: [BMLR](https://bookdown.org/roback/bookdown-BeyondMLR/ch-logreg.html) 6.2, 6.5 <li>Count regression: [BMLR](https://bookdown.org/roback/bookdown-BeyondMLR/ch-poissonreg.html) 4.2, 4.4, 4.9</ul> |
| 3 | Generalized Linear Models (GLMs): Multinomial and Ordinal Logistic Regressions | <ul><li>[Faraway:](https://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwbV1LT8MwDLZgu2wXoIDoGFPgPtZH-og0Ia3TJi5cEOIaNV1yGRRp3fj9OOlDLeqpSquqdVo7n53PNoDvPTvzfzbBVSFVmfAYFaGQKfWEEhnNZKBUlO7KpNcWVafOltYkS51f1xCmu2zpRUWX7o0box-AWCTi6M-fBw5tmhsgQGCoWT5ldcWnejyGcVrs0bag3TkWHcjZSsnX6872EoZSJyNcwZnMLbioICOpFLKwYPzWlF3F0UhDx7Ly8jU8opuJvzExvW4KogOuZPmdHvYv78uFOd7AZLv5WL_O8bG8iuNw1L1Y98W4hUH-k8s7INR1d652EphyqYoi4SsnZqFy_EBIXHlseGoJxH-_zAZswTtS20BqObm5XrFC-SZZV3Nog9XzIjZM22fr3TIehyGLAzrpvekeRgg5gjKIMYXB8XCSD2Z6Z-YDzWC4WiXJ5x9w-aQv) Chapter 5</ul> |
| 4 | Linear Mixed-Effects Models | <ul><li> Initial motivation: [ISL](https://www.statlearning.com) 3.3. Potential Problems (*Correlation of Error Terms*) <li>[BMLR](https://bookdown.org/roback/bookdown-BeyondMLR/ch-beyondmost.html) from 8.1 to 8.8 </ul>|
| 5 | Survival Analysis |See Kleinbaum and Klein (2005) in **Reference Material** |
| 6 | Missing Data | See van Buuren, S. (2012) in **Reference Material** |
| 7 | Quantile Regression | <ul><li>[Fahrmeir (2013)](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=-K7&J=TC0000904267&P=Link&PT=EZProxy&H=d91b1366d8&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Flink.springer.com%2F10.1007%2F978-3-642-34333-9) 10. Quantile Regression (except 10.2.2 Bayesian Quantile Regression) </ul>|
| 8 | Local and Robust Regressions | <ul><li> [ISL](https://www.statlearning.com) 7.2 Step Functions <li>[ISL](https://www.statlearning.com) 7.6 Local Regression <li> [Rousseeuw and Leroy (2003)](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=ZEEST&J=TC0000239030&P=Link&PT=EZProxy&H=48e3fef958&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fonlinelibrary.wiley.com%2Fdoi%2Fbook%2F10.1002%2F0471725382) 1. Introduction <li > [Rousseeuw and Leroy (2003)](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=ZEEST&J=TC0000239030&P=Link&PT=EZProxy&H=48e3fef958&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fonlinelibrary.wiley.com%2Fdoi%2Fbook%2F10.1002%2F0471725382) 2. Simple Regression </ul>|

## Deliverables

This is an __assignment-based course__. The following deliverables will determine your course grade:

| Assessment       | Weight  | 
| :---:            | :---:   |
| Lab Assignment 1 | 15%     |
| Lab Assignment 2 | 15%     |
| Lab Assignment 3 | 15%     |
| Lab Assignment 4 | 15%     |
| Quiz 1           | 20%     |
| Quiz 2           | 20%     |

## Lectures

### Schedule

| Day                  | Tuesday            | Thursday         |
| :---:                | :---:             | :---:           |
| Time                 | 11:00 a.m. to 12:20 p.m. (PST)    | 11:00 a.m to 12:20 p.m. (PST) |
| Room                 | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408) | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408) |
| Lecture instructor       | Alexi Rodríguez-Arelis     | Alexi Rodríguez-Arelis | 
| Teaching Assistant | Siddhesh Khandelwal  | Yulia Egorova | 

## Labs

### Schedule

|                      | **L01**             | **L02**           |  
| :---:                | :---:             | :---:           |
| **Day**                  | Thursday            | Wednesday         |
| **Time**                 | 1:00 - 2:50 (PST)    | 2:00 - 3:50 p.m. (PST)  |
| **Room**                 | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)           | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)         |
| **Lab instructor**       | Alexi Rodríguez-Arelis      | Alexi Rodríguez-Arelis | 
| **Teaching Assistants**   | Mohamad Amin Mohamadi and Alireza Naderi       | Yulia Egorova and Katie Florko | 

### Lab Topics and Due Dates

|      | **Lab Topic**        | **Due Date**         |
| :---:| :---:            | :---:            |
| **1**    | Introduction to Generalized Linear Models<br>(Lectures 1 and 2) | 2022-01-15 6:00 p.m. (PST) |
| **2**    | Categorical and Mixed-Effects Regression Models<br>(Lectures 3 and 4) | 2022-01-22 6:00 p.m. (PST) |
| **3**    | Survival Analysis and Missing Data<br>(Lectures 5 and 6) | 2022-01-29 6:00 p.m. (PST) |
| **4**    | Quantile, Robust, and Local Regressions<br>(Lectures 7 and 8) | 2022-02-05 6:00 p.m. (PST) |

## Quizzes

See [calendar](https://ubc-mds.github.io/calendar/).

## Office hours

|       | **Office hour 1** | **Office hour 2** | **Office hour 3** | **Office hour 4** | **Office hour 5** | **Office hour 6** | **Office hour 7** |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Day**   | Monday | Tuesday | Wednesday | Thursday | Thursday | Friday | Friday | 
| **Time**  | 4:00 - 5:00 p.m. (PST) | 4:00 - 5:00 p.m. (PST) | 4:00 - 5:00 p.m. (PST) | 5:00 - 6:00 p.m. (PST) | 6:00 - 7:00 p.m. (PST) | 1:00 - 2:00 p.m. (PST) | 5:00 - 6:00 p.m. (PST) |
| **Room**  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  | [Virtual](https://canvas.ubc.ca/courses/83553/external_tools/15408)  |
| **Person**  | Shuyi | Alireza | Siddhesh | Yulia | Alexi | Katie | Amin |

See [calendar](https://ubc-mds.github.io/calendar/) for the most up to date information.

## Reference Material
- Agresti, A (2012). *Categorical Data Analysis*, John Wiley & Sons, Incorporated. ProQuest Ebook Central.
    - The e-book is available through the [UBC Library](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=ZEEST&J=TC0000182416&P=Link&PT=EZProxy&H=af1255a89f&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fonlinelibrary.wiley.com%2Fdoi%2Fbook%2F10.1002%2F0470114754). You can obtain a PDF copy with your CWL account. This book is helpful for generalized linear models with discrete responses.
- Collett, D. (2003). *Modelling Binary Data (2nd ed.)*. Chapman and Hall/CRC. https://doi.org/10.1201/b16654
    - The e-book is available through the [UBC Library](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=JTX&J=TC0001459465&P=Link&PT=EZProxy&H=a796b2aeda&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fwww.taylorfrancis.com%2Fbooks%2F9780429129087).
- Dambolena, I. G., Eriksen, S. E., and Kopcso, D. P. (2009). [Logarithmic transformations in regression: Do you transform back correctly?](https://login.ezproxy.library.ubc.ca/login?url=https://www.tandfonline.com/doi/pdf/10.1080/10511970802234976?needAccess=true) *PRIMUS : Problems, Resources, and Issues in Mathematics Undergraduate Studies*, 19(3), 280-295.
- Fahrmeir, L. (2013). *Regression Models, Methods and Aplications*. Springer Berlin Heidelberg.
    - The e-book is available through the [UBC Library](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=-K7&J=TC0000904267&P=Link&PT=EZProxy&H=d91b1366d8&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Flink.springer.com%2F10.1007%2F978-3-642-34333-9). You can obtain a PDF copy with your CWL account.
- Faraway, Julian J. (2014). *Linear Models with `R`*, CRC Press LLC. ProQuest Ebook Central.
    - The e-book is available through the [UBC Library](https://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwbV1LT8MwDLZgu2wXoIDoGFPgPtZH-og0Ia3TJi5cEOIaNV1yGRRp3fj9OOlDLeqpSquqdVo7n53PNoDvPTvzfzbBVSFVmfAYFaGQKfWEEhnNZKBUlO7KpNcWVafOltYkS51f1xCmu2zpRUWX7o0box-AWCTi6M-fBw5tmhsgQGCoWT5ldcWnejyGcVrs0bag3TkWHcjZSsnX6872EoZSJyNcwZnMLbioICOpFLKwYPzWlF3F0UhDx7Ly8jU8opuJvzExvW4KogOuZPmdHvYv78uFOd7AZLv5WL_O8bG8iuNw1L1Y98W4hUH-k8s7INR1d652EphyqYoi4SsnZqFy_EBIXHlseGoJxH-_zAZswTtS20BqObm5XrFC-SZZV3Nog9XzIjZM22fr3TIehyGLAzrpvekeRgg5gjKIMYXB8XCSD2Z6Z-YDzWC4WiXJ5x9w-aQv). You can obtain a PDF copy with your CWL account. This book is great for learning how to work within the `R` environment with the models we will be working on. Its approach is essentially practical.     
- Gelman, A. and Hill, J. (2007). *Data Analysis Using Regression and Multilevel/Hierarchical Models*. Analytical Methods for Social Research. Cambridge University Press.
    - The physical book is available through the [UBC Library](http://webcat2.library.ubc.ca/vwebv/search?searchArg=Data%20analysis%20using%20regression%20and%20multilevel%2Fhierarchical%20models%20%2F&searchCode=TALL&searchType=1). This book is pretty useful and practical as introductory material.
- James, G., Witten, D., Hastie, T., and Tibshirani, R. (2014). [*An Introduction to Statistical Learning: with Applications in `R`*](https://www.statlearning.com). Springer Publishing Company, Incorporated.
- Kleinbaum, D. G. and Klein, M. (2005). *Survival analysis : A Self-Learning Text*. Springer.
    - The e-book is available through the [UBC Library](https://ezproxy.library.ubc.ca/login?auth=shibboleth&url=https://link.springer.com/10.1007/0-387-29150-4). This book is a good start for Survival Analysis:
        - **Chapter 1 (Introduction):** Introduction to Survival Analysis (I), Censored Data (II), Terminology and Notation (III).
        - **Chapter 2 (Kaplan-Meier Curves):** Review (I), Example of Kaplan-Meier Curves (II), General Features of  Kaplan-Meier Curves (III), Confidence Intervals for Kaplan-Meier Curves (VII and VIII).
        - **Chapter 3 (Cox Proportional Hazards Model):** Example of Cox Proportional Hazards Model (I), Formula of Cox Proportional Hazards Model (II), Why the Cox Proportional Hazards Model is Popular (III), Estimation of the Cox Proportional Hazards Model (IV).
        - **Chapter 7 (Parametric Model):** Overview (I), Relationship Between the Probability Density Function with Hazard and Survival Functions (II), Weibull Example (IV).
- Rousseeuw, L. P. J. and Leroy A. M. (2003). *Robust Regression and Outlier Detection*. Hoboken, NJ : Wiley-Interscience.
    - The e-book is available through the [UBC Library](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=ZEEST&J=TC0000239030&P=Link&PT=EZProxy&H=48e3fef958&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fonlinelibrary.wiley.com%2Fdoi%2Fbook%2F10.1002%2F0471725382). You can obtain a PDF copy with your CWL account.
- Roback, P. and  Legler, J. (2020). [*Beyond Multiple Linear Regression*](https://bookdown.org/roback/bookdown-BeyondMLR/).
- Rubin, D. B. (1987). *Multiple Imputation for Nonresponse in Surveys*. Wiley.
    - The e-book is available through the [UBC Library](https://gw2jh3xr2c.search.serialssolutions.com/log?L=GW2JH3XR2C&D=ZEEST&J=TC0000340639&P=Link&PT=EZProxy&H=6c88ebd0c3&U=https%3A%2F%2Fezproxy.library.ubc.ca%2Flogin%3Furl%3Dhttps%3A%2F%2Fonlinelibrary.wiley.com%2Fdoi%2Fbook%2F10.1002%2F9780470316696). You can obtain a PDF copy with your CWL account.
- van Buuren, S. (2012). [*Flexible Imputation of Missing Data*](https://stefvanbuuren.name/fimd/):
    - **1.1 The problem of missing data.**
    - **1.2 Concepts of MCAR, MAR and MNAR.**
    - **1.3 Ad-hoc solutions.**
    - **1.4 Multiple imputation in a nutshell.**

## Recommended Course Reviews

This course is entirely taught in `R` (we will follow the [`tidyverse` style guide](https://style.tidyverse.org/index.html)) with a reasonable mathematical and statistical basis. We strongly recommend reviewing the following courses:

- *DSCI 551: Descriptive Statistics and Probability for Data Science*, for basic statistical concepts and familiarity with the mathematical notation.
- *DSCI 552: Statistical Inference and Computation I*, for statistical inference concepts with a frequentist approach.
- *DSCI 561: Regression I*, since the topics of this course follow the same thread.
- *DSCI 531: Data Visualization I*, for plotting tools using the package `ggplot2`.
    
## Dataset References 

These are the papers from which each dataset used in the lectures comes from. If you are interested in knowing more about them, you can obtain a PDF copy of each paper with your CWL account via the UBC library:

- Brockmann, H.J. (1996). [Satellite Male Groups in Horseshoe Crabs, Limulus polyphemus](https://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwrV3JasMwEBUlpZBLl7Sl6YY_oE4sy5sgFEpICKU9NadcjFYSmtghCyRf0t-tJC_EPhRaepMHS8jSSPM0M3oGALkdx67tCYRyKV0GacCp9CBX60RCySMcYiigy2qpOq_F1ZiMLqL0v-mFYrZvvd4JXXcPEnOUZbU1z6W-fxdoh6eO-XQUvDyGCnXrbK_hxCkDDCHKgs9KH20FelDOR_pzWxXbdYhljTEanoF10e8iC6V2SbDK9Pg_H3gOTnPsar1kynYBjkTSAs1yC923wMkkNaVL8NVbkNXn8wcxjJ8b0euaZysTvyuzVJUYH9i6Kpsl1ijVOSbTtPZ2f6V6nYuectnbbLGdb2tNLNP5fjkVi1J-BcbDwbg_svOfQNhMIRdsu4KHEnIsIiQYJoGQvsKQmAuOsE8lojRnrPEIlZQHHIUEEs8PBVHQjaJr0EjSRNwAS8ebmMNk4DHkRYgQSt2ARoxRnzuhJG2AitmNlxnVR3x4REI41sMf6-GP8-GPd20QmVn7RZV4MB7p0u3fq96BZpY-rn1B96CxWW3FgyGOeDR6_g1rIQSN). *Ethology*, 102: 1-21.
- Deb, P. and Trivedi, P. (1997). [Demand for medical care by the elderly: a finite mixture approach](https://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwnV1tS8MwEA5uftAvvk6cL6N_oK5L0pfJUEr34gQZ4j75JaZLCsOtzqng_os_1kuTDjsVwU-lF9oL5Mg9x909hxDBZ469cick3G0GggcJ9YXHSUIDb6RyXn6DgsPmcqVUx89bY1SVZVYmmCX1AS_FE1nHOHCxiy9nz7aaHqWyrGaURgmVwEI1Te7yPlYM7BpLEtvHLi54IF2E-AWZUuNautvoId9FXlOy0vJX5G38x3Z30JaBnVao7WQXrcl0D23kXckv--ijNeXzx4u2nPJUtOrZi6VlAGstk88pLqjepaIkXlgAKK2OGv09WZi1c7MYWt2xQrjFT27G7yqJURSGhuncSCto2O0MoyvbTG6wAT4Ejg0xVSAVdTyn2PeJkBC4yKRBhUdHHuFurPphMSAzAXCPOwnAGgHOWkoVrwEoPUDl9CmVh6rySgDkGIlmTByaSCfmIwExYRx7SSBjX1bRID9MNtP8HEwzMWPG7vpRX6XYmwxgnMtUTY0DD8wIIw3CWNhvs-uwQ6kDEodFA4ZZr4oq2REuf2fOr4puMxv5puYPLT8qMZKjX3Qdo01Nk6sKK09Q-XX-Jk8zXogaWm9H94NeLbPxT5yWAM4). *Journal of Applied Econometrics*, 12(3), 313-336.
- Grunfeld Y. (1958). [The determinants of corporate investment](https://www.proquest.com/docview/301899386?pq-origsite=summon&accountid=14656). Ph.D. thesis, Department of Economics, University of Chicago.
- Harrison, D. and Rubinfeld, D.L. (1978). [Hedonic prices and the demand for clean air](http://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwnV07T8MwELYQDLDwKCDeyghDaOy0TixVSICourBVYrRc50wBNVRtQeLfc-fEpYAQiMF5nB9JbOf8Obn7zFgqzpP4i04wgANV7iQgPC-gZTOligRsAiYRhfWLOSya6pz_8EOfyyZhgjiRSp5m-RmteClj0sBpm5NBV-_2aq6H88QvLTfPEBznfijk88BE9pkWQd-nMWplAmOwC-NPd4PdBS-eYHjyxS_wG7njH59pk63XkDS6rPrQFluCssFWg8fytMF2bz684TBhrQ6m22zWGZnJ00UPCiLY7TT9WTR8JmP6-6iKHBNr0TTEmbKIEHLWcQWMUBDiED7XcrwNUwZxJTIPk1qww_rdm_51L66XcYh5KomtVGZGtJwcEO-NQplVvCDqQwlKcGvBtp2yhjxghZFu4KRSTqZcDFomFZDusuXyuYQ9FqlMICISMLA0L3WpqrhpXAvz2MLl-ywOTajHFVmHDlZsVMea6lhnufZ1rAWmD-38x_RZ6Ay6BigV8NDYor_kvPR9Z34ZAHgEqmT9qlPTxvCGgeOcHncPdIhhjCHnWKrQw9no4N9XP2Rr3DMp05ejI7Y8m7zAsaeZOPGvjN9evwO2Ww2r). *Journal of Environmental Economics and Management*, 5, 81–102.
- Henderson, H. V. and McCulloch, C. E. (1990). [Transform or link?](https://ecommons.cornell.edu/bitstream/handle/1813/31620/BU-1049-MA.pdf;jsessionid=1E54532D482EC351824111A78C797021?sequence=1). *Biometrics Unit Technical Reports; Number BU-1049-MA*.
- Mangasarian, O. L., Street, W. N., and Wolberg, W. H. (1995). [Breast cancer diagnosis and prognosis via linear programming](http://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwlV1Nb9QwEB2xPSA4tHQLohRKDoDgsDSJndiRKlApVBx74PNk2bGDKui2jbf8Ff4uM46tbpZKFZdIO55NvNLLeLx-8waAla_z2UpMEAZXtlZKzllZGSk7WTBdtDa3ts6N61aoOnUqjSGWZaAJhkN9zJfML7dHCi-yfnt-MaPmUXTIGjtpTGAi2cDr-rKkvFsPbQwYBpyafxsvQMTDbPEOVxE5yQSH8iZKHH2iKv4TrsMadLQBKk03kU9WagPHAo___7vuwXpMT7ODAU-bcMvNp3A7seOnsJG6QGQxKEzh7pKk4RQ2o91nL6Oi9ast-LN_qvufb94RAX6xvxc-ZIPtkFDXj23vB_rfiR-b9dxmx_3ZdUO_T_TYgFtsfIXHtuOBinaK84wD9-Hz0YdPhx9nsSPEDPeBJWmp6pJ3VS1tzlvR8Ua6WljWlm3RaMkMs52R1jmJWGu4a6wwtugaaauGtQWaH8Da_GzuHkJWVlpwbgpthKOz3aZsmeRWC9mJxnG7DS8STNT5IPyhaMOEO0xF_WkUZ4qrSuTomEB0k-MzgpiK3UXx4un_F_9DX3qvDjCPw2yPMbxfcCPwLXrd6lgngdMmqa5lx6cJqyoiNTzQLz3xeRq4YWZbAYxXXgGJ27CT8K5iZPOqJEFAUnl8dP2XduDOUPVPjObHsLboL92TIGmxCxPx9TteMcDshnf0L2aRR50). *Operations Research*, 43(4), 570-577.
- Wolberg, W. H. and Mangasarian, O. L. (1990). [Multisurface method of pattern separation for medical diagnosis applied to breast cytology](https://libkey.io/libraries/498/articles/35797998/full-text-file?utm_source=api_542). *Proceedings of the National Academy of Sciences of the United States of America*, 87(23), 9193–9196.
- Wood, P. (1967). [Algebraic Model of the Lactation Curve in Cattle](https://ubc.summon.serialssolutions.com/2.0.0/link/0/eLvHCXMwfV1LS8NAEF6kIHhRW98voic9xGYzyW4WilCqxYN4ED2XzXRXim2qrRX99242SW0i7TGzEwiZycw3zOQbQsC_9txKTIg8yYw_U2awHBUyFIwr1JE0RZEG3sfKqM7FkoY-RE3fQBQWSFulc56WW0-Pt39DHRXe5YJuduHGcgJK5zDRgLs5k-ZCduluZWuKpgVvwvdP9a-_f9SNK554m2zmINNpZ15RJ2sqaZB1O-yJ0wap5x_01LnMWaevdshHayQnbzft4WvaSh5gq2mvnUycrkwblkVj7Rjw6DxIzLr55dPObPKlyqJB4nQsZXIu3iUv3bvnzr2b72Nw0WR5z6WxgV_UZ5iCCm1qF8VBMlTgaRUjgKAKgcUgI_SBa8H6QkrsM8Yx5MA57JFaMk7UAXGCCEMQ0gQ3oYKYU6GFBMG0L1CHmseH5LwwUu89o93o2XY5RL3ifRqdwnordPYzs841ipOjpSfHZMOEJZ4mKBqckNrnZKZOLSnDmXW2X2pLzng). *Nature*, 216, 164–165.
    
## Policies

See the general [MDS policies](https://ubc-mds.github.io/policies/).

## Attribution
    
The course is built upon previous years' materials developed by previous instructors.

## Dealing With COVID-19

The [COVID-19 pandemic](https://www.who.int/emergencies/diseases/novel-coronavirus-2019/events-as-they-happen) has affected us all in different ways: it is okay to not be okay, and we all need to support each other during this time. With that said:

- Our (virtual) door is always open, please feel free to talk to us about how you are doing and if/how we can help you (and if we cannot help you, we can point you in the direction of someone who can).
- You do not ever need to explain yourself. If you need support, need to miss a class, or need extra time for an assignment, just ask.
- UBC has [great student support resources](https://students.ubc.ca/covid19) related to COVID-19 (and otherwise).

### Covid Safety at UBC

**Masks:** Masks are required indoors, including in classrooms, as per the [BC Public Health Officer orders](https://www2.gov.bc.ca/gov/content/covid-19/info/restrictions#masks). For the purposes of this order, the term "masks" refers to medical and non-medical masks that cover our noses and mouths. Masks are a primary tool to make it harder for COVID-19 to find a new host. You will need to wear a medical or non-medical mask anytime you are indoors at UBC, for your own protection, and the safety and comfort of everyone else in the class. Please do not eat in the classroom. If you need to drink water/coffee/tea/etc., please keep your mask on between sips. Please note that there are some people who cannot wear a mask. These individuals are equally welcome in our class. 

**Vaccination:** If you have not yet had a chance to get vaccinated against COVID-19, vaccines are available to you, free, and on campus (you can find more information [here](http://www.vch.ca/covid-19/covid-19-vaccine)). The higher the rate of vaccination in our community overall, the lower the chance of spreading this virus. You are an important part of the UBC community. Please arrange to get vaccinated if you have not already done so. 

**COVID-19 testing:** UBC will require COVID-19 testing for all students, faculty and staff, with exemptions provided for those who are vaccinated against COVID-19. You can find more information [here](https://news.ubc.ca/2021/08/26/ubc-implements-vaccine-declaration-and-rapid-testing-for-covid-19/).

**Your personal health:**
If you are sick, it is important that you stay home – no matter what you think you may be sick with (e.g., cold, flu, other). A daily self-health assessment is required before attending campus. Every day, before leaving home, complete the self-assessment for COVID-19 symptoms [using this tool](https://bc.thrive.health/covid19/en).

Stay home if you have COVID-19 symptoms, have recently tested positive for COVID-19, or are required to quarantine. You can check [this website](http://www.bccdc.ca/health-info/diseases-conditions/covid-19/self-isolation#Who) to find out if you should self-isolate or self-monitor. 

Your precautions will help reduce risk and keep everyone safer. In this class, the marking scheme is intended to provide flexibility so that you can prioritize your health and still be able to succeed: 
- all course notes will be provided online,
- all worksheets and lab assignments can be done and handed in online,
- all quizzes will be held online/in-person,
- live class recordings will be streamed and archived for later viewing online, and
- office hours will be held online/in-person.

## Official statement from UBC regarding the online learning experience:

>*During this pandemic, the shift to online learning has greatly altered teaching and studying at UBC, including changes to health and safety considerations. Keep in mind that some UBC courses might cover topics that are censored or considered illegal by non-Canadian governments. This may include, but is not limited to, human rights, representative government, defamation, obscenity, gender or sexuality, and historical or current geopolitical controversies. If you are a student living abroad, you will be subject to the laws of your local jurisdiction, and your local authorities might limit your access to course material or take punitive action against you. UBC is strongly committed to academic freedom, but has no control over foreign authorities (please visit [http://www.calendar.ubc.ca/vancouver/index.cfm?tree=3,33,86,0](http://www.calendar.ubc.ca/vancouver/index.cfm?tree=3,33,86,0) for an articulation of the values of the University conveyed in the Senate Statement on Academic Freedom). Thus, we recognize that students will have legitimate reason to exercise caution in studying certain subjects. If you have concerns regarding your personal situation, consider postponing taking a course with manifest risks, until you are back on campus or reach out to your academic advisor to find substitute courses. For further information and support, please visit: [http://academic.ubc.ca/support-resources/freedom-expression](http://academic.ubc.ca/support-resources/freedom-expression).*
