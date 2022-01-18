
<!-- README.md is generated from README.Rmd. Please edit that file -->

# regexciteklv

<!-- badges: start -->
<!-- badges: end -->

The goal of regexciteklv is to make regular expressions more exciting!
It provides convenience functions to make some common tasks with string
manipulation and regular expressions a bit easier.

## Installation

You can install the development version of regexciteklv from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("Kingslin0810/kingslin-toyrpkgfoo")
```

## Usage

A fairly common task when dealing with strings is the need to split a
single string into many parts. This is what `base::strplit()` and
`stringr::str_split()` do.

``` r
(x <- "alfa,bravo,charlie,delta")
#> [1] "alfa,bravo,charlie,delta"
strsplit(x, split = ",")
#> [[1]]
#> [1] "alfa"    "bravo"   "charlie" "delta"
stringr::str_split(x, pattern = ",")
#> [[1]]
#> [1] "alfa"    "bravo"   "charlie" "delta"
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(regexciteklv)
str_split_one(x, pattern = ",")
#> [1] "alfa"    "bravo"   "charlie" "delta"
```
