# Format issues list from GH

Format issues list from GH

## Usage

``` r
gh_issue_fmt(
  i,
  which = c("title", "number", "body", "labels", "url", "created", "updated",
    "gh_user_issue")
)
```

## Arguments

- i:

  List of issues from
  [`gh_issue_fetch()`](https://docs.ropensci.org/promoutils/reference/gh_issue_fetch.md)

- which:

  Which fields to include

## Value

Issues formated as a data frame

## Examples

``` r
i <- gh_issue_fetch(owner = "ropensci", repo = "weathercan")
i <- gh_issue_fmt(i, which = "title")
i
#> # A tibble: 6 × 1
#>   title                                                                         
#>   <chr>                                                                         
#> 1 weather_dl errors when downloading small batches of recent data with an out o…
#> 2 Vision and best practices                                                     
#> 3 Review vignettes                                                              
#> 4 Vignette: Homogenizing ECCC Data from weathercan                              
#> 5 Add package vision                                                            
#> 6 Add French localisation                                                       
```
