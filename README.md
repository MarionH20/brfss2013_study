# Exploring the BRFSS 2013 Data

Introductory statistics project in R: exploring CDC BRFSS 2013 health survey data with descriptive statistics, conditional probability, a simulation-based test and correlation.

## Project Overview

This is the final project for the Coursera course "Introduction to Probability and Data with R" (Duke University).

The Behavioral Risk Factor Surveillance System (BRFSS) is a collaborative project between all US states, participating US territories and the Centers for Disease Control and Prevention (CDC). Its objective is to collect uniform, state-specific data on preventive health practices and risk behaviors linked to chronic diseases, injuries and preventable infectious diseases in the adult population (description adapted from the [CDC BRFSS website](https://www.cdc.gov/brfss/)).

This study analyzes the BRFSS data from 2013, focusing on three research questions.

## Repository Contents

```         
brfss2013_study/
├── LICENSE.md
├── README.md
├── brfss2013_study.Rmd      (analysis: code and text)
└── docs/
    └── index.html      (the knitted report)
```

Open [`index.html`](https://marionh20.github.io/brfss2013_study/) to read the report. The data file is not included (see below).

## Research Questions

1.  Is the obesity rate lower with higher education?
2.  Is income associated with education, sex and race?
3.  Is physical activity associated with vegetable consumption?

## Data

The data file `brfss2013_clean.RData` is not provided with this project. To re-run the analysis you need to build your own version of this file. See the "Load data" section of the notebook for details. The raw BRFSS data are available on the [CDC website](https://www.cdc.gov/brfss/annual_data/annual_2013.html).

## Methodology

**Methods:** descriptive statistics, conditional probabilities, simulation-based hypothesis test, Spearman correlation.

**Tools:** R, `dplyr`, `ggplot2`.

**Limitations:** - This is an observational study, so it does not allow causal conclusions. - To keep the analysis simple, the sampling weights are not used. To reduce error and bias, within-group proportions are compared instead of absolute figures. - Income is a household income category. Several variables are self-reported so they can contain systematic errors (over- or understatement etc)

## Key Findings

1.  Adults who graduated from college or technical school have a lower obesity rate than the rest of the population.
2.  Respondents with higher income categories tend to have a higher educational level.
    - For the lowest (did not graduate from high school) and the highest educational level (graduated from college or technical school), men tend to have a higher household income than women.
    - For respondents with marital status "Divorced", "Widowed" or "Separated", men tend to have a higher household income than women.
    - For a similar educational level, the category "White" tends to have a higher income than the category "Black or African American".
3.  A higher consumption of vegetables is weakly associated with a higher level of physical activity.

## Acknowledgements

Thanks to Coursera and Duke University for providing the BRFSS data set and the framework for this study. Thanks to the CDC for sharing valuable data and documentation about the BRFSS over the years.

## License

See `LICENSE.md`. It applies to the code and text of this project, not to the BRFSS data.

## Author / Contact

**Marion Houliere** [linkedin.com/in/marionhouliere](https://www.linkedin.com/in/marionhouliere)
