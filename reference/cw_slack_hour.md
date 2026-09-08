# Schedule 1-hour before messages on rOpenSci Slack

Will only work if running between the time that the 1-week message was
posted and the start of the coworking.

## Usage

``` r
cw_slack_hour(
  user = "UNRAUCMTK",
  test_run = FALSE,
  dry_run = FALSE,
  print = FALSE,
  call = rlang::caller_env()
)
```

## Arguments

- user:

  Character. Slack user id.

- test_run:

  Logical. Whether to run a test of this message posting to the test
  channel.

- dry_run:

  Logical. Whether to do a dry run, print the message only.

- print:

  Logical. Whether to simply print the text to console instead of
  copying to the clipboard.

- call:

  Environment. Parent environment for messaging.

## Value

Nothing

## Examples

``` r
if (FALSE) { # interactive()
cw_slack_hour(test_run = TRUE)
cw_slack_hour(dry_run = TRUE)
}
```
