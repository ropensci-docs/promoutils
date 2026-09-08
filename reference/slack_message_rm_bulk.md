# Bulk remove Slack messages

Use with caution! This removes all messages matched by timestamp `ts` in
`channel` or `channel_id`. Note that users can only delete their own
messages.

## Usage

``` r
slack_message_rm_bulk(msg, channel = NULL, channel_id = NULL, ts = NULL)
```

## Arguments

- msg:

  Data frame. Output of `slack_messages` containing messages to remove.
  Should contain columns "channel" and "ts". Removes all messages.

- channel:

  Character. Channel Name. Not required if channel_id supplied.

- channel_id:

  Character. Channel id.

- ts:

  Numeric. Timestamp to identify message to remove

## Value

Nothing. Side effect of removing message from channel
