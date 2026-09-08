# Remove a Slack message

Use with caution! Note that users can only delete their own messages. If
you try to delete another user's message you will get a "Cant Delete
Message" message from the Slack API.

## Usage

``` r
slack_message_rm(msg = NULL, channel = NULL, channel_id = NULL, ts = NULL)
```

## Arguments

- msg:

  Data frame. Output of `slack_messages` containing message to remove.
  Should contain columns "channel" and "ts". Note that only the most
  recent message will be removed.

- channel:

  Character. Channel Name. Not required if channel_id supplied.

- channel_id:

  Character. Channel id.

- ts:

  Numeric. Timestamp to identify message to remove (if no `msg`)

## Value

Nothing. Side effect of removing message from channel

## See also

[`slack_message_rm_bulk()`](https://docs.ropensci.org/promoutils/reference/slack_message_rm_bulk.md)
