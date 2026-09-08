# Fetch issues from a GH repository

Fetches issues from a GitHub repository and returns them as a list. Pass
on to
[`gh_issue_fmt()`](https://docs.ropensci.org/promoutils/reference/gh_issue_fmt.md)
for formatting.

## Usage

``` r
gh_issue_fetch(
  state = "open",
  labels = NULL,
  since = NULL,
  owner = "rosadmin",
  repo = "scheduled_socials",
  issue = NULL,
  verbose = FALSE
)
```

## Arguments

- state:

  Character. Which issues to fetch: "open", "closed", "all"

- labels:

  Character vector. Fetch only issues with these labels. (Optional)

- since:

  Character/Date/datetime. Fetch only issues since this date/time.
  (Optional)

- owner:

  Character. Owner of the repository

- repo:

  Character. Name of the repository (name of the package)

- issue:

  Numeric. Specific Issue number to fetch.

- verbose:

  Logical. Show extra informative messages.

## Value

List of issues

## Examples

``` r
i <- gh_issue_fetch(owner = "ropensci", repo = "weathercan")
#> ⠙ 6 items, page 1 | 2ms
i <- gh_issue_fetch(owner = "ropensci", repo = "weathercan", verbose = TRUE)
#> ℹ owner: ropensci; repo: weathercan
```
