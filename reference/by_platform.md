# Arrange by platform

Arranges data in long by platform (linkedin and mastodon).

## Usage

``` r
by_platform(df)
```

## Arguments

- df:

  Data frame. Formatted data including social media handles.

## Value

Data frame arranged by platform on which to advertise.

## Examples

``` r
if (FALSE) { # interactive()
u <- uc_fetch() |>
  uc_fmt("2025-01-01") |>
  uc_handles() |>
  by_platform()
}
```
