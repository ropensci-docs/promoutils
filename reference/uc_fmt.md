# Extract out resource information

Extract out resource information

## Usage

``` r
uc_fmt(uc, min_date, pkgs = NULL)
```

## Arguments

- uc:

  Data frame. Data frame of usecases from
  [`uc_fetch()`](https://docs.ropensci.org/promoutils/reference/uc_fetch.md).

- min_date:

  Character/Date. Minimum date of usecases to retain.

- pkgs:

  Data frame. Optional data frame of package details (defaults to
  [`pkgs_ru()`](https://docs.ropensci.org/promoutils/reference/pkgs_ru.md)).

## Value

Data frame of formatted use cases.

## Examples

``` r
if (FALSE) { # interactive()
u <- uc_fetch() |>
  uc_fmt("2025-01-01")
u
}
```
