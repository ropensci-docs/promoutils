# Add social media handles

Add social media handles

## Usage

``` r
uc_handles(uc, force_masto = FALSE)
```

## Arguments

- uc:

  Data frame. Formatted use cases output of
  [`uc_fmt()`](https://docs.ropensci.org/promoutils/reference/uc_fmt.md).

- force_masto:

  Logical. Passed to
  [`monarch::add_handles()`](https://rdrr.io/pkg/monarch/man/add_handles.html).
  Whether or not to force a re-check of mastodon handles (good if you
  think they've changed or they are 'none' and you want to check again).

## Value

Data frame with social media handles appended/filled in

## Examples

``` r
if (FALSE) { # interactive()
u <- uc_fetch() |>
  uc_fmt("2025-01-01") |>
  uc_handles()
}
```
