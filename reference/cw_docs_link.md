# Get link to Coworking docs

Creates the coworking doc if it doesn't exist and returns a link either
way. Optionally creates PR adds link to event page.

## Usage

``` r
cw_docs_link(which = "next", open_sites = TRUE, add = FALSE)
```

## Arguments

- which:

  Character/Date. "next" to fetch details on the next coworking session,
  "last" to fetch details on the last scheduled (in future) coworking
  session, or a Date fetch details for a specific coworking session.

- open_sites:

  Logical. Open websites with relevant details?

- add:

  Logical. Whether to initialize a PR and add the link to the events
  file.

## Value

Google Docs link
