# Create help-wanted `socials_post_issue()` command

Create help-wanted
[`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
command

## Usage

``` r
help_post(help, date_time = NULL, dry_run = FALSE, print = FALSE)
```

## Arguments

- help:

  Data frame. Formatted help-wanted issues including social media
  handles and arranged by platform upon which to post, output of
  [`by_platform()`](https://docs.ropensci.org/promoutils/reference/by_platform.md).

- date_time:

  Character/Date. When to post. Defaults to next Thursday if `NULL`.

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
h <- help_fetch("2025-05-23") |>
  help_handles() |>
  by_platform()

help_post(h, print = TRUE)  # For non-interactive examples
}
```
