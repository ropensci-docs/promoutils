# Review blogposts views for Throwback Thursday highlights

Use
[`matomo_update()`](https://docs.ropensci.org/promoutils/reference/matomo_update.md)
and friends to download and update blog post view data. `tt_review()`
summarizes the posts by view and optionally filters to a specific month.

## Usage

``` r
tt_review(which_month = NULL)
```

## Arguments

- which_month:

  Numeric. Which month to return? Numeric 1-12 for month. Default `NULL`
  returns all.

## Value

Data frame of posts by views with urls

## Examples

``` r
if (FALSE) { # dir.exists(matomo_dir())
tt_review(11)
}
```
