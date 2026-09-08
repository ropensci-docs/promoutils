# Get the next post date/time

Finds the next date/time to post by day of the week and hour.

## Usage

``` r
post_time(day, hour)
```

## Arguments

- day:

  Character. Day of the week (e.g., "Monday")

- hour:

  Numeric. Hour at which to post (e.g., 8)

## Value

Date time as character (without timezone)

## Examples

``` r
post_time("Wednesday", 8)
#> [1] "2026-09-09 08:00:00"
```
