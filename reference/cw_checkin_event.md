# Create draft message for checking in with Cohosts about the Event review

When an event has been drafted use this draft text to invite the
cohost(s) to review via Slack or Email.

## Usage

``` r
cw_checkin_event(which = "next", names = NULL, print = FALSE)
```

## Arguments

- which:

  Character/Date. "next" to fetch details on the next coworking session,
  "last" to fetch details on the last scheduled (in future) coworking
  session, or a Date fetch details for a specific coworking session.

- names:

  Character. Names of cohost if overriding those in the event listing.

- print:

  Logical. Whether to print the copied text to the console.

## Examples

``` r
if (FALSE) { # interactive()
cw_checkin_event("2026-04-07")
}
```
