# Delete a scheduled message

Removes a currently scheduled messages. Can only be removed by
scheduler.

## Usage

``` r
slack_scheduled_rm(msg = NULL, channel = NULL, id = NULL)
```

## Arguments

- msg:

  Data frame. Output of `slack_list_scheduled()` containing messages to
  remove. Should contain columns "channel" and "id"

- channel:

  Character. If no msg, the Channel of the message to be deleted.

- id:

  Character. If no msg, the ID of the message to be deleted.

## Value

Nothing

## Examples

``` r
if (FALSE) { # interactive()
# Schedule message
slack_posts_write("Testing delete msg", when = (Sys.Date() + lubridate::days(2)))

# Confirm scheduled
slack_scheduled_list()

# Remove message
slack_scheduled_list() |>
  dplyr::filter(text == "Testing delete msg") |>
  slack_scheduled_rm()

# Confirm that removed
slack_scheduled_list()

if (FALSE) { # \dontrun{
slack_scheduled_rm(channel = "#testing-api", id = "Q08U4S3J6QG")
} # }
}
```
