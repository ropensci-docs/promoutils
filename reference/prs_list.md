# List PRs

List open PRs by url, title and number, optionally matching to a title
or branch name (ref)

## Usage

``` r
prs_list(match = NULL, owner = "ropensci", repo = "roweb3")
```

## Arguments

- match:

  Character. String to match in the title or branch name

- owner:

  Character. GitHub owner of the repository (defaults to 'ropensci')

- repo:

  Character. GitHub repository name (defaults to 'roweb3')

## Value

Data frame with PR url, number, title, and branch name ('ref')

## Examples

``` r
prs_list("coworking") # List all coworking related (open) PRs
#> ⠙ 12 items, page 1 | 2ms
#> # A tibble: 1 × 4
#>   html_url                                     number title                ref  
#>   <chr>                                         <int> <chr>                <chr>
#> 1 https://github.com/ropensci/roweb3/pull/1358   1358 Add November 2026 C… cowo…
```
