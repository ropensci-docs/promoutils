# Convert an api url to a user-facing url

When working with the GitHub api, urls are often in for the api.

## Usage

``` r
url_from_api(url)
```

## Arguments

- url:

  Character. URL to convert

## Value

User-facing url character string

## Examples

``` r
url_from_api("https://api.github.com/repos/ropensci/qualtRics/issues/386")
#> [1] "https://github.com/ropensci/qualtRics/issues/386"
```
