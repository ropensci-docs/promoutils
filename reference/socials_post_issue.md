# Create a draft issue to post to Mastodon and LinkedIn

Formats the body and title of an issue and posts it on
"rosadmin/scheduled_socials". The issue will bed opened in a browser for
editing and confirmation. Note that issues will not be posted until the
labels "draft" and "needs-review" have been removed.

## Usage

``` r
socials_post_issue(
  time,
  tz = "America/Winnipeg",
  title,
  body,
  where = "mastodon",
  avoid_dups = TRUE,
  add_hash = TRUE,
  dry_run = FALSE,
  open_browser = TRUE,
  over_char_limit = cli::cli_abort,
  verbose = FALSE
)
```

## Arguments

- time:

  Date/time. Date and time at which the post should be made

- tz:

  Character. Timezone (from
  [`OlsonNames()`](https://rdrr.io/r/base/timezones.html)) in which to
  post

- title:

  Character. Title of the post (`[Post]` and the date will be prepended
  and appended

- body:

  Character. Text to be posted (omit the YAML for posting info; \#RStats
  and @rstats@a.gup.pe will be appended for Mastodon, \#RStats for
  LinkedIn), *or* link to text file with both Mastodon and LinkedIn body
  text, headed by by —- Mastodon —– and — LinkedIn —–.

- where:

  Character vector. Either `mastodon` and/or `linkedin` to specify which
  platforms this should be posted on.

- avoid_dups:

  Logical. Don't post an issue if any open issue has the same title.

- add_hash:

  Logical. Whether to automatically add the RStats hashtags.

- dry_run:

  Logical. Whether to perform a dry run (do not post, but display draft
  if `verbose = TRUE`).

- open_browser:

  Logical. Whether to open the issue in the browser.

- over_char_limit:

  Function. Error or warn if over the character limit?

- verbose:

  Logical. Show extra informative messages.

## Examples

``` r
socials_post_issue("2025-01-01 00:00:00",
                   title = "test post",
                   body = "Test body",
                   dry_run = TRUE, verbose = TRUE)
#> 
#> ── Post to mastodon [DRY RUN] ──
#> 
#> title: [Post] - test post - 2025-01-01
#> labels: mastodon, draft, and needs-review
#> body:
#> ~~~
#> time: 2025-01-01 00:00:00
#> tz: America/Winnipeg
#> ~~~
#> Test body
#> 
#> #RStats
#> @rstats@a.gup.pe
```
