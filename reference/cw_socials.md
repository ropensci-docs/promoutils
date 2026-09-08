# Create a draft post for coworking

Creates draft posts for Mastodon and LinkedIn (by opening issues on
rosadmin/scheduled_socials) and Slack (by printing the post text and
schedule).

## Usage

``` r
cw_socials(
  date,
  who_masto,
  who_slack,
  who_linkedin,
  who_main_masto = "@steffilazerte@fosstodon.org",
  who_main_slack = "<@UNRAUCMTK>",
  who_main_linkedin = "Steffi LaZerte",
  posters_tz = "America/Winnipeg",
  test_run = FALSE,
  dry_run = FALSE,
  print = TRUE,
  branch = NULL
)
```

## Arguments

- date:

  Character/Date. Date of the coworking event (local)

- who_masto:

  Character. The full mastodon handle for the cohost (i.e.
  `XXXX@XXXX.com`)

- who_slack:

  Character. The full API Slack id for the cohost (i.e. `<@UXXXXXXX>`)

- who_linkedin:

  Character. The full LinkedIn handle for the cohost (i.e. `@XXXX`)

- who_main_masto:

  Character. The full mastodon handle for the rOpenSci staff organizer.

- who_main_slack:

  Character. The Slack id for the rOpenSci staff organizer (i.e.,
  `<@UXXXXXXX>`. Defaults to Steffi's id.

- who_main_linkedin:

  Character. The full LinkedIn handle for the rOpenSci staff organizer.

- posters_tz:

  Character. Timezone of poster. Required for getting the time at which
  to post Slack messages as these are posted in the local timezone

- test_run:

  Logical. Whether to do a test run (i.e. post to a test area).

- dry_run:

  Logical. Whether to do a dry run (i.e. don't post).

- print:

  Logical. Whether to simply print the text to console instead of
  copying to the clipboard.

- branch:

  Character. Branch name if not on main.

## Examples

``` r
cw_socials("2023-07-04",
           who_masto = "@cohost@mastodon.org",
           who_linkedin = "Cohost the Best",
           who_slack = "<UXXXXXXX>",
           dry_run = TRUE)
#> 
#> ── Coworking - Timezone: Europe/Paris ──────────────────────────────────────────
#> 
#> ── Post to mastodon [DRY RUN] ──
#> 
#> title: [Post] - Coworking Jul 2023 - week before - 2023-06-27
#> labels: mastodon, draft, and needs-review
#> body:
#> ~~~
#> time: 2023-06-27 14:00:00
#> tz: Europe/Paris
#> ~~~
#> Coworking and Office Hours next week!
#> 
#> Theme: Create/Update your 'Happy File'/'Brag Document'!
#> 
#> Tuesday July 4th 14:00 Europe Central (12:00 UTC)
#> 
#> Join @cohost@mastodon.org and @steffilazerte@fosstodon.org
#> 
#> - General coworking
#> - Explore what goes into a 'Happy File'/'Brag Document' and why you need one
#> - Start collecting items to add to your 'Happy File'
#> - Chat with Maëlle and other attendees and discuss our theme!
#> 
#> https://ropensci.org/events/coworking-2023-07
#> 
#> #RStats
#> @rstats@a.gup.pe
#> 
#> ── Post to mastodon [DRY RUN] ──
#> 
#> title: [Post] - Coworking Jul 2023 - 1-hr before - 2023-07-04
#> labels: mastodon, draft, and needs-review
#> body:
#> ~~~
#> time: 2023-07-04 13:00:00
#> tz: Europe/Paris
#> ~~~
#> rOpenSci Coworking and Office Hours coming up in an hour!
#> 
#> Today's Theme: Create/Update your 'Happy File'/'Brag Document'! with cohost
#> @cohost@mastodon.org
#> 
#> Tuesday July 4th 14:00 Europe Central (12:00 UTC)
#> 
#> https://ropensci.org/events/coworking-2023-07
#> 
#> #RStats
#> @rstats@a.gup.pe
#> 
#> ── Post to linkedin [DRY RUN] ──
#> 
#> title: [Post] - Coworking Jul 2023 - week before - 2023-06-27
#> labels: linkedin, draft, and needs-review
#> body:
#> ~~~
#> time: 2023-06-27 14:00:00
#> tz: Europe/Paris
#> ~~~
#> Coworking and Office Hours next week!
#> 
#> Theme: Create/Update your 'Happy File'/'Brag Document'!
#> 
#> Tuesday July 4th 14:00 Europe Central (12:00 UTC)
#> 
#> Join Cohost the Best and Steffi LaZerte
#> 
#> - General coworking
#> - Explore what goes into a 'Happy File'/'Brag Document' and why you need one
#> - Start collecting items to add to your 'Happy File'
#> - Chat with Maëlle and other attendees and discuss our theme!
#> 
#> https://ropensci.org/events/coworking-2023-07
#> 
#> #RStats
#> 
#> ── Post to linkedin [DRY RUN] ──
#> 
#> title: [Post] - Coworking Jul 2023 - 1-hr before - 2023-07-04
#> labels: linkedin, draft, and needs-review
#> body:
#> ~~~
#> time: 2023-07-04 13:00:00
#> tz: Europe/Paris
#> ~~~
#> rOpenSci Coworking and Office Hours coming up in an hour!
#> 
#> Today's Theme: Create/Update your 'Happy File'/'Brag Document'! with cohost
#> Cohost the Best
#> 
#> Tuesday July 4th 14:00 Europe Central (12:00 UTC)
#> 
#> https://ropensci.org/events/coworking-2023-07
#> 
#> #RStats
#> 
#> ── Slack Dry Run ──
#> 
#> • When: 2023-06-27 07:00:00 America/Winnipeg
#> • Where: #general
#> • What: Join us for Social Coworking and office hours next week!
#> :grey_exclamation: Theme: Create/Update your 'Happy File'/'Brag Document'!
#> :hourglass_flowing_sand: When: Tuesday July 4th 14:00 Europe Central (12:00
#> UTC) :cookie: Hosted by: <@UNRAUCMTK> and co-host <UXXXXXXX> :mag: Details:
#> https://ropensci.org/events/coworking-2023-07 You can use this time for... -
#> General coworking - Explore what goes into a 'Happy File'/'Brag Document' and
#> why you need one - Start collecting items to add to your 'Happy File' - Chat
#> with <UXXXXXXX> and other attendees about our theme!
#> 
#> ── Slack Dry Run ──
#> 
#> • When: 2023-06-27 07:00:00 America/Winnipeg
#> • Where: #co-working
#> • What: Join us for Social Coworking and office hours next week!
#> :grey_exclamation: Theme: Create/Update your 'Happy File'/'Brag Document'!
#> :hourglass_flowing_sand: When: Tuesday July 4th 14:00 Europe Central (12:00
#> UTC) :cookie: Hosted by: <@UNRAUCMTK> and co-host <UXXXXXXX> :mag: Details:
#> https://ropensci.org/events/coworking-2023-07 You can use this time for... -
#> General coworking - Explore what goes into a 'Happy File'/'Brag Document' and
#> why you need one - Start collecting items to add to your 'Happy File' - Chat
#> with <UXXXXXXX> and other attendees about our theme!
#> rOpenSci's next Social Coworking and office hours is up in two weeks :tada:
#> 
#> These are casual online events for coworking and socializing generally centred on a theme related to R and tools for open/reproducible science.
#> You can work quietly on your own, join in a discussion, or work while listening to the discussion, what ever suits you (and you don't have to follow the theme).
#> 
#> :grey_exclamation: Theme: Create/Update your 'Happy File'/'Brag Document'!
#> :hourglass_flowing_sand: When: Tuesday July 4th 14:00 Europe Central (12:00 UTC)
#> :cookie: Hosted by: @Steffi LaZerte and co-host @Cohost the Best
#> :mag: Details: https://ropensci.org/events/coworking-2023-07
#> 
#> You can use this time for...
#> - General coworking
#> - Explore what goes into a 'Happy File'/'Brag Document' and why you need one
#> - Start collecting items to add to your 'Happy File'
#> - Chat with @Cohost the Best and other attendees about our theme!
#> ℹ Post on 2023-06-20 07:00:00

if (FALSE) { # \dontrun{
cw_socials("2023-07-04", who_masto = "@cohost@mastodon.org", who_slack = "<UXXXXXXX>")
} # }
```
