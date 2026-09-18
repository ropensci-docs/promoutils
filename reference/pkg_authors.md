# Get package author names

Get package author names

## Usage

``` r
pkg_authors(package, pkgs)
```

## Arguments

- package:

  Character. Package name

- pkgs:

  Data frame. Packages returned by
  [`pkgs_ru()`](https://docs.ropensci.org/promoutils/reference/pkgs_ru.md).

## Value

Character name of maintainer

## Examples

``` r
pkg_authors("weathercan", pkgs_ru())
#> [1] "Steffi LaZerte"
```
