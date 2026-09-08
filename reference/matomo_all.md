# Download all Matomo historic views

Downloads all views from a specific year range (2010-2024 by defautl).
Views can be read with
[`matomo_read()`](https://docs.ropensci.org/promoutils/reference/matomo_read.md).

## Usage

``` r
matomo_all(year_range = 2010:2024, host = "https://ropensci.matomo.cloud")
```

## Arguments

- year_range:

  Numeric vector. Years to download views for.

- host:

  Character. URL for the Matomo host to collect views for. Defaults to
  that of rOpenSci.

## Value

Nothing. Writes views to disk.

## Details

Requires a Renviron "MATOMO_TOKEN" key representing your token for
Matomo for the host you'd like to fetch data for.
