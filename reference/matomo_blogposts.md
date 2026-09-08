# Formats and filter Matomo views to blogposts

Formats and filter Matomo views to blogposts

## Usage

``` r
matomo_blogposts(views)
```

## Arguments

- views:

  Data frame from
  [`matomo_read()`](https://docs.ropensci.org/promoutils/reference/matomo_read.md).

## Value

Data frame of blog post views

## Examples

``` r
if (FALSE) { # dir.exists(matomo_dir())
matomo_read() |>
  matomo_blogposts()
}
```
