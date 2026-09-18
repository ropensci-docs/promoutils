# Create a draft event for coworking

Creates a draft coworking event for the roweb3 website. All details
pulled from the coworking todo list issue in `rosadmin/comms`. See
[`cw_issue()`](https://docs.ropensci.org/promoutils/reference/cw_issue.md).

## Usage

``` r
cw_event(date, dry_run = FALSE)
```

## Arguments

- date:

  Character/Date. Date of the coworking event to create

- dry_run:

  Logical. Whether to really create the event or just return the text.
