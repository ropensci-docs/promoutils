# List of packages and details from R-Universe API

List of packages and details from R-Universe API

## Usage

``` r
pkgs_ru(universe = "ropensci")
```

## Arguments

- universe:

  Character. Universe to collect details from.

## Value

Data frame of package details

## Examples

``` r
pkgs_ru()
#> # A tibble: 364 × 16
#>    package    title           owner url   docs  maintainer_name maintainer_email
#>    <chr>      <chr>           <chr> <chr> <chr> <chr>           <chr>           
#>  1 sasquatch  "Use 'SAS', R,… rope… http… http… Ryan Zomorrodi  rzomor2@uic.edu 
#>  2 babeldown  "Helpers for A… rope… http… http… Maëlle Salmon   msmaellesalmon@…
#>  3 gigs       "Assess Fetal,… rope… http… http… Simon R Parker  simon.parker147…
#>  4 tesseract  "Open Source O… rope… http… http… Jeroen Ooms     jeroenooms@gmai…
#>  5 npi        "Access the U.… rope… http… http… Frank Farach    frank.farach@gm…
#>  6 rfishbase  "R Interface t… rope… http… http… Carl Boettiger  cboettig@gmail.…
#>  7 osmapiR    "'OpenStreetMa… rope… http… http… Joan Maspons    joanmaspons@gma…
#>  8 pkgcheck   "Package Check… rope… http… http… Mark Padgham    mark.padgham@em…
#>  9 osmplotr   "Bespoke Image… rope… http… http… Mark Padgham    mark.padgham@em…
#> 10 osmextract "Download and … rope… http… http… Andrea Gilardi  andrea.gilardi@…
#> # ℹ 354 more rows
#> # ℹ 9 more variables: maintainer_github <chr>, maintainer_linkedin <chr>,
#> #   maintainer_orcid <chr>, maintainer_description <chr>,
#> #   maintainer_uuid <int>, contributors <list>, maintainer_mastodon <chr>,
#> #   maintainer_bluesky <chr>, maintainer_twitter <chr>
```
