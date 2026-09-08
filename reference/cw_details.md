# Fetch details about coworking sessions

Fetch details about coworking sessions

## Usage

``` r
cw_details(which = "next")
```

## Arguments

- which:

  Character/Date. "next" to fetch details on the next coworking session,
  "last" to fetch details on the last scheduled (in future) coworking
  session, or a Date fetch details for a specific coworking session.

## Value

Data frame with coworking event details

## Examples

``` r
if (FALSE) { # interactive()
cw_details()
# cw_details("2023-11") # Only works for events in the future
}
```
