# Create use case `socials_post_issue()` command

Create use case
[`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
command

## Usage

``` r
uc_post(uc, date_time = NULL, dry_run = FALSE, print = FALSE)
```

## Arguments

- uc:

  Data frame. Formatted use cases including social media handles and
  arranged by platform upon which to post, output of `uc_platform()`.

- date_time:

  Character/Date. When to post. Defaults to next Wednesday if `NULL`.

- dry_run:

  Logical. Whether to do a dry run (i.e. don't post).

- print:

  Logical. Whether to simply print the text to console instead of
  copying to the clipboard.

## Value

Copies commands to clipboard, optionally prints if (`print = TRUE`).

## Examples

``` r
if (FALSE) { # interactive()
u <- uc_fetch() |>
  uc_fmt("2025-01-01") |>
  uc_handles() |>
  by_platform()

uc_post(u, dry_run = TRUE,print = TRUE)
}
```
