
# azmet-qa-dashboard

<!-- badges: start -->
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

<!-- badges: end -->

This report has two types of validations: 1) rule-based validations and 2) forecast-based validations.  Rule-based validations check if values are within ranges, are correct relative to one another, and are not out of range for certain numbers of observations.  Forecast-based validations start with creating a timeseries model of the data back to 2003.  These models are updated and used to forecast the current day.  The observed data is then compared to the forecast data, and if they are very different the data is flagged.

## Reproducibility

This project uses [`renv`](https://rstudio.github.io/renv/articles/renv.html) for package management. When opening this repo as an RStudio Project for the first time, `renv` should automatically install itself and prompt you to run `renv::restore()` to install all package dependencies.

## Collaboration guidelines

To contribute to this project, please create a new branch for your changes and make a pull request. One easy way to do this from within R is with the `usethis` package and the `pr_*` functions. `pr_init("branch-name")` begins a new branch locally, `pr_push()` helps you create a new pull request, and after it is merged you can use `pr_finish()` to clean things up. More about this workflow [here](https://usethis.r-lib.org/articles/pr-functions.html).
