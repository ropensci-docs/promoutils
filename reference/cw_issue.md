# Create Coworking To-Dos

Create a GitHub issue in a repository listing the Coworking ToDos. If no
date or timezone, picks the next appropriate date (first Tuesday of the
month following an existing coworking issue) and next appropriate
timezone (cycling through America, Europe, and Australia) automatically.

## Usage

``` r
cw_issue(
  date = NULL,
  tz = NULL,
  theme = "XXXX",
  cohost = "XXXX",
  repo = "rosadmin/comms",
  dry_run = FALSE
)
```

## Arguments

- date:

  Character. Date of next event (if NULL picks next first Tuesday).

- tz:

  Character. Timezone of next event (if NULL picks next in order).

- theme:

  Character. Name of theme, if unknown, uses XXXX placeholder

- cohost:

  Character. Name of cohost, if unknown, uses XXXX placeholder

- repo:

  Character. GitHub repository including owner (e.g., `rosadmin/comms`)

- dry_run:

  Logical. Whether to really create the issue or just return the text.

## Value

Nothing

## Examples

``` r
if (FALSE) { # interactive()
cw_issue(dry_run = TRUE)
}
```
