# Get the last 100 messages from a channel

Requires one of `channel` OR `channel_id`

## Usage

``` r
slack_messages(channel = NULL, channel_id = NULL)
```

## Arguments

- channel:

  Character. Channel Name. Not required if channel_id supplied.

- channel_id:

  Character. Channel id.

## Value

Data frame. Messages and details

## Examples

``` r
if (FALSE) { # interactive()
slack_messages(channel_id = "C026GCWKA") # General
slack_messages(channel = "General")
}
```
