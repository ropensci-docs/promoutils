# Get social media handles for helpwanted issues

Get social media handles for helpwanted issues

## Usage

``` r
help_handles(help, force_masto = FALSE)
```

## Arguments

- help:

  Data frame of help wanted issues.

- force_masto:

  Logical. Passed to
  [`monarch::add_handles()`](https://rdrr.io/pkg/monarch/man/add_handles.html).
  Whether or not to force a re-check of mastodon handles (good if you
  think they've changed or they are 'none' and you want to check again).

## Value

Data frame of help wanted issues with social median handles added

## Examples

``` r
if (FALSE) { # interactive()
h <- help_fetch("2025-01-01") |>
  help_handles()
}
```
