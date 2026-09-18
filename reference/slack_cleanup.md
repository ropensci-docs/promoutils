# Clean up old scheduled messages

Removes previously scheduled messages from `#admin-scheduled` if after
the posting date. Only removes messages scheduled by current user.

## Usage

``` r
slack_cleanup()
```

## Value

Nothing

## Examples

``` r
if (FALSE) { # interactive()

slack_posts_write("testing cleanup",
                  when = Sys.time() + lubridate::seconds(600),
                  tz = Sys.timezone())
slack_scheduled_list()

slack_cleanup()
}
```
