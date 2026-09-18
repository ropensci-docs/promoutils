# Fetch help wanted issues

Fetch help wanted issues

## Usage

``` r
help_fetch(min_date, json = "/repos/rosadmin/help-wanted/contents/issues.json")
```

## Arguments

- min_date:

  Character/Date. Earliest date a help-wanted label was added to an
  issue to be included.

- json:

  Character. Location of the issues.json file to use.

## Value

Data frame of help wanted issues

## Examples

``` r
if (FALSE) { # interactive()
h <- help_fetch("2025-01-01")
}
```
