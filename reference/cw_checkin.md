# Create draft message for checking in with Cohosts

The week before, prepare the slides and coworking document, then use
this draft text to invite the cohost(s) to review via Slack or Email.

## Usage

``` r
cw_checkin(which = "next", names = NULL, print = FALSE)
```

## Arguments

- which:

  Character/Date. "next" to fetch details on the next coworking session,
  "last" to fetch details on the last scheduled (in future) coworking
  session, or a Date fetch details for a specific coworking session.

- names:

  Character. Names of cohost if overriding those in the event listing.

- print:

  Logical. Whether to simply print the text to console instead of
  copying to the clipboard.
