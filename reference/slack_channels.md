# List channels and their ids

List channels and their ids

## Usage

``` r
slack_channels(channel = NULL, types = c("public_channel", "private_channel"))
```

## Arguments

- channel:

  Character. Channel Name.

- types:

  Character. Type of channels, one or both of "public_channel" or
  "private_channel"

## Value

Data frame of channel names, ids, types, descriptions, and topics. Or if
`channel` provided, a single channel id.

## Examples

``` r
if (FALSE) { # interactive()
slack_channels()
slack_channels("general")
chn <- slack_channels(types = "private_channel")
}
```
