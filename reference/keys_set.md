# Set keys required for promoutils API access

This function guides uses through the finding and setting tokens so that
promoutils can find them.

## Usage

``` r
keys_set(type = NULL)
```

## Arguments

- type:

  Character Vector. Keys/tokens to set ("slack", "matomo", "linkedin",
  "github").

## Value

Nothing, side effect of setting token credentials in the keyring or via
`gitcreds::gitcres_set()` for GitHub tokens.
