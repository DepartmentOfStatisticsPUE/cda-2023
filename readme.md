# Categorical Data Analysis 2022/23

## Description of the data

Source:

+ id -- company identifier
+ woj -- region (województwo) id (02, 04, ..., 32)
+ public -- is the company public (1) or private (0)?
+ size -- size of the company (small = up tp 9 employees, medium = 10 to 49, big = over 49)
+ nace -- NACE (PKD) sections (1 letter)
+ nace_division -- NACE (PKD) division (2-digits, https://www.biznes.gov.pl/pl/klasyfikacja-pkd) 
+ vacancies -- how many vacancies the company reported?

Sample rows from the dataset

```r
           id woj public   size nace nace_division vacancies
    1:  27350  14      1  Large    O            84         2
    2:  26705  14      1  Large    O            84         1
    3: 257456  24      1  Large    O            84         2
    4: 183657  16      1 Medium    O            84         0
    5: 200042  18      1 Medium    O            84         0
   ---                                                      
57476: 244800  08      1 Medium    P            85         0
57477:  62309  08      1 Medium    R            93         0
57478: 106708  08      0 Medium    B            08         0
57479:  62264  08      0 Medium    B            08         0
57480: 255865  08      0  Small    C            23         0
```

## Outline of lecture

1.  Discrete distributions [[code for/from
    lecture](https://htmlpreview.github.io/?https://github.com/DepartmentOfStatisticsPUE/cda-2023/blob/main/notebooks/01-distributions.html)]
2.  Maximum Likelihood Estimation (MLE) [[code for/from
    lecture](https://htmlpreview.github.io/?https://github.com/DepartmentOfStatisticsPUE/cda-2023/blob/main/notebooks/02-mle.html)]
3.  Goodness of fit (GoF) [[code for/from
    lecture](https://htmlpreview.github.io/?https://github.com/DepartmentOfStatisticsPUE/cda-2023/blob/main/notebooks/03-gof.html)]
4. Contingency tables:
    + Simpson's paradox [[code for/from lecture](https://htmlpreview.github.io/?https://github.com/DepartmentOfStatisticsPUE/cda-2023/blob/main/notebooks/04-simpson-paradox.html)]
    + Contingency tables and Cramer's V [[code for/from lecture](https://htmlpreview.github.io/?https://github.com/DepartmentOfStatisticsPUE/cda-2023/blob/main/notebooks/05-ctables.html)]

## Required packages / modules

-   R:
    -   `distributions3`,
    -   `maxLik`, `rootSolve`
    - `vcd`, `fitdistrplus`
-   Python:
    -   `scipy`, `numpy`, `pandas`
    - `pingouin`, `matplotlib`, `statsmodels`
-   Julia:
    -   `Distributions.jl`, `DataFrames.jl`,
    -   `Optim.jl`, `Roots.jl`
    - `HypothesisTests.jl`, `StatsBase.jl`
    - `FreqTables.jl`, `CSV.jl`

## Software versions

``` r
R version 4.2.2 (2022-10-31)
```

``` python
Python 3.10.7 (v3.10.7:6cc6b13308, Sep  5 2022, 14:02:52)
```

``` julia
Julia Version 1.9.0-rc1
Commit 3b2e0d8fbc1 (2023-03-07 07:51 UTC)
```
