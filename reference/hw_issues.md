# Create help wanted JSON file

Function created for rosadmin/help-wanted. Fetches package repos with
issues labelled help-wanted (and variants). Saves output to issues.json
for use by helpwanted workflows including
https://ropensci.org/help-wanted.

## Usage

``` r
hw_issues(
  min_date = Sys.Date() - lubridate::years(2),
  throttle = 10/60,
  path = "issues.json",
  verbose = TRUE
)
```

## Arguments

- min_date:

  Date. Fetch issues since this data.

- throttle:

  Numeric. Maximum requests per second. Default throttled to 10 requests
  per minute which is the max rate for unauthenticated GitHub Pats (i.e.
  on GH actions).

- path:

  Character. Filename/path to save json of issues to.

- verbose:

  Logical. Show extra informative messages.

## Value

Creates/updates issues json list at `path`

## Examples

``` r
if (FALSE) { # interactive()
hw_issues()
}
```
