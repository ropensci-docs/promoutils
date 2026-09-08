# Update Matomo views

Update a specific year of Matomo blog views. Defaults to current year.
Views can be read with
[`matomo_read()`](https://docs.ropensci.org/promoutils/reference/matomo_read.md).

## Usage

``` r
matomo_update(
  year = lubridate::year(Sys.Date()),
  host = "https://ropensci.matomo.cloud"
)
```

## Arguments

- year:

  Numeric. Year to update

- host:

  Character. URL for the Matomo host to collect views for. Defaults to
  that of rOpenSci.

## Value

Nothing. Updates views to disk.

## Details

Requires a .Renviron "MATOMO_TOKEN" key representing your token for
Matomo for the host you'd like to fetch data for.
