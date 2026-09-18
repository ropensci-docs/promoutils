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
#>    package      title         owner url   docs  maintainer_name maintainer_email
#>    <chr>        <chr>         <chr> <chr> <chr> <chr>           <chr>           
#>  1 bibtex       Bibtex Parser rope… http… http… James Joseph B… balamut2@illino…
#>  2 gert         Simple Git C… r-lib http… http… Jeroen Ooms     jeroenooms@gmai…
#>  3 babelquarto  Renders a Mu… rope… http… http… Maëlle Salmon   msmaellesalmon@…
#>  4 opencv       Bindings to … rope… http… http… Jeroen Ooms     jeroenooms@gmai…
#>  5 frictionless Read and Wri… fric… http… http… Peter Desmet    peter.desmet@in…
#>  6 osmextract   Download and… rope… http… http… Andrea Gilardi  andrea.gilardi@…
#>  7 pkgcheck     Package Chec… rope… http… http… Mark Padgham    mark.padgham@em…
#>  8 osmapiR      'OpenStreetM… rope… http… http… Joan Maspons    joanmaspons@gma…
#>  9 phruta       Phylogenetic… rope… http… http… Cristian Roman… cromanpa@arizon…
#> 10 fluidsynth   Read and Pla… rope… http… http… Jeroen Ooms     jeroenooms@gmai…
#> # ℹ 354 more rows
#> # ℹ 9 more variables: maintainer_github <chr>, maintainer_mastodon <chr>,
#> #   maintainer_linkedin <chr>, maintainer_twitter <chr>,
#> #   maintainer_description <chr>, maintainer_uuid <int>,
#> #   maintainer_orcid <chr>, contributors <list>, maintainer_bluesky <chr>
```
