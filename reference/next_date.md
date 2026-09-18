# Find the next date

Given a date and a day of the week, Given a date return the next month's
first Tuesday

## Usage

``` r
next_date(month, which = "Tues", n = 1, call = rlang::caller_env())
```

## Arguments

- month:

  Character/Date. The current month. Date returned is the next month.

- which:

  Character/Numeric. Which week day to return. Either number or
  abbreviated English weekday.

- n:

  Numeric. The nth week to return (i.e. the 1st Tuesday if `n = 1` and
  `which = "Tues"`).

- call:

  Environment. Calling environment for appropriate messages if used
  within another function.

## Value

A date

## Examples

``` r

# Get the next first Tuesday
next_date("2023-11-01")
#> [1] "2023-12-05"
next_date("2023-11-30")
#> [1] "2023-12-05"

# Get the next 3rd Tuesday
next_date("2023-11-01", n = 3)
#> [1] "2023-12-19"

# Oops
if (FALSE) { # \dontrun{
next_date("2023-11-01", n = 5)
} # }
```
