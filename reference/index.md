# Package index

## API authentication helpers

- [`keys_check()`](https://docs.ropensci.org/promoutils/reference/keys_check.md)
  : Key status of credentials
- [`keys_set()`](https://docs.ropensci.org/promoutils/reference/keys_set.md)
  : Set keys required for promoutils API access

## Coworking Helpers

- [`cw_checkin()`](https://docs.ropensci.org/promoutils/reference/cw_checkin.md)
  : Create draft message for checking in with Cohosts
- [`cw_checkin_event()`](https://docs.ropensci.org/promoutils/reference/cw_checkin_event.md)
  : Create draft message for checking in with Cohosts about the Event
  review
- [`cw_details()`](https://docs.ropensci.org/promoutils/reference/cw_details.md)
  : Fetch details about coworking sessions
- [`cw_docs_link()`](https://docs.ropensci.org/promoutils/reference/cw_docs_link.md)
  : Get link to Coworking docs
- [`cw_event()`](https://docs.ropensci.org/promoutils/reference/cw_event.md)
  : Create a draft event for coworking
- [`cw_issue()`](https://docs.ropensci.org/promoutils/reference/cw_issue.md)
  : Create Coworking To-Dos
- [`cw_slack_hour()`](https://docs.ropensci.org/promoutils/reference/cw_slack_hour.md)
  : Schedule 1-hour before messages on rOpenSci Slack
- [`cw_slides_link()`](https://docs.ropensci.org/promoutils/reference/cw_slides_link.md)
  : Open and fetch link to coworking slides
- [`cw_socials()`](https://docs.ropensci.org/promoutils/reference/cw_socials.md)
  : Create a draft post for coworking

## Announcement Helpers

- [`uc_fetch()`](https://docs.ropensci.org/promoutils/reference/uc_fetch.md)
  : Fetch and format use cases from a GitHub Discussion board

- [`uc_fmt()`](https://docs.ropensci.org/promoutils/reference/uc_fmt.md)
  : Extract out resource information

- [`uc_handles()`](https://docs.ropensci.org/promoutils/reference/uc_handles.md)
  : Add social media handles

- [`uc_post()`](https://docs.ropensci.org/promoutils/reference/uc_post.md)
  :

  Create use case
  [`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
  command

- [`help_fetch()`](https://docs.ropensci.org/promoutils/reference/help_fetch.md)
  : Fetch help wanted issues

- [`help_handles()`](https://docs.ropensci.org/promoutils/reference/help_handles.md)
  : Get social media handles for helpwanted issues

- [`help_post()`](https://docs.ropensci.org/promoutils/reference/help_post.md)
  :

  Create help-wanted
  [`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
  command

- [`tt_post()`](https://docs.ropensci.org/promoutils/reference/tt_post.md)
  :

  Create Throwback Thursday
  [`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
  command

- [`tt_review()`](https://docs.ropensci.org/promoutils/reference/tt_review.md)
  : Review blogposts views for Throwback Thursday highlights

- [`hw_issues()`](https://docs.ropensci.org/promoutils/reference/hw_issues.md)
  : Create help wanted JSON file

## API functions

- [`slack_channels()`](https://docs.ropensci.org/promoutils/reference/slack_channels.md)
  : List channels and their ids
- [`slack_cleanup()`](https://docs.ropensci.org/promoutils/reference/slack_cleanup.md)
  : Clean up old scheduled messages
- [`slack_message_rm()`](https://docs.ropensci.org/promoutils/reference/slack_message_rm.md)
  : Remove a Slack message
- [`slack_message_rm_bulk()`](https://docs.ropensci.org/promoutils/reference/slack_message_rm_bulk.md)
  : Bulk remove Slack messages
- [`slack_messages()`](https://docs.ropensci.org/promoutils/reference/slack_messages.md)
  : Get the last 100 messages from a channel
- [`slack_posts_write()`](https://docs.ropensci.org/promoutils/reference/slack_posts_write.md)
  : Write Slack message
- [`slack_scheduled_list()`](https://docs.ropensci.org/promoutils/reference/slack_scheduled_list.md)
  : List currently scheduled messages
- [`slack_scheduled_rm()`](https://docs.ropensci.org/promoutils/reference/slack_scheduled_rm.md)
  : Delete a scheduled message
- [`slack_user()`](https://docs.ropensci.org/promoutils/reference/slack_user.md)
  : Fetch details on a specific user
- [`slack_users()`](https://docs.ropensci.org/promoutils/reference/slack_users.md)
  : Fetch a list of Slack users
- [`li_auth()`](https://docs.ropensci.org/promoutils/reference/li_auth.md)
  : Authorize rOpenSci client with LinkedIn
- [`li_posts_read()`](https://docs.ropensci.org/promoutils/reference/li_posts_read.md)
  : Get a list of recent posts by rOpenSci
- [`li_posts_write()`](https://docs.ropensci.org/promoutils/reference/li_posts_write.md)
  : Post to LinkedIn
- [`li_urn_me()`](https://docs.ropensci.org/promoutils/reference/li_urn_me.md)
  : Fetch your personal URN number
- [`matomo_all()`](https://docs.ropensci.org/promoutils/reference/matomo_all.md)
  : Download all Matomo historic views
- [`matomo_blogposts()`](https://docs.ropensci.org/promoutils/reference/matomo_blogposts.md)
  : Formats and filter Matomo views to blogposts
- [`matomo_dir()`](https://docs.ropensci.org/promoutils/reference/matomo_dir.md)
  : Cache folder to store matomo views
- [`matomo_read()`](https://docs.ropensci.org/promoutils/reference/matomo_read.md)
  : Read Matomo views saved to disk
- [`matomo_update()`](https://docs.ropensci.org/promoutils/reference/matomo_update.md)
  : Update Matomo views

## Dictionary/Wordlist Helpers (in progress…)

- [`dict_helpwanted()`](https://docs.ropensci.org/promoutils/reference/dict_helpwanted.md)
  : Dictionary for help-wanted
- [`dict_usecases()`](https://docs.ropensci.org/promoutils/reference/dict_usecases.md)
  : Dictionary for usecases
- [`wordlist_create()`](https://docs.ropensci.org/promoutils/reference/wordlist_create.md)
  : Create Word lists for spelling dictionaries
- [`wordlist_update()`](https://docs.ropensci.org/promoutils/reference/wordlist_update.md)
  : Add specific words to the wordlist

## GitHub issues

- [`gh_issue_close()`](https://docs.ropensci.org/promoutils/reference/gh_issue_close.md)
  : Close a GH issue
- [`gh_issue_fetch()`](https://docs.ropensci.org/promoutils/reference/gh_issue_fetch.md)
  : Fetch issues from a GH repository
- [`gh_issue_fmt()`](https://docs.ropensci.org/promoutils/reference/gh_issue_fmt.md)
  : Format issues list from GH
- [`gh_issue_post()`](https://docs.ropensci.org/promoutils/reference/gh_issue_post.md)
  : Create a GH issues post

## Utility functions

- [`ro_urn`](https://docs.ropensci.org/promoutils/reference/ro_urn.md) :
  rOpenSci linkedin organization URN
- [`by_platform()`](https://docs.ropensci.org/promoutils/reference/by_platform.md)
  : Arrange by platform
- [`.gh_cache()`](https://docs.ropensci.org/promoutils/reference/dot-gh_cache.md)
  : Create a cached version of the GH api calls
- [`next_date()`](https://docs.ropensci.org/promoutils/reference/next_date.md)
  : Find the next date
- [`pkg_authors()`](https://docs.ropensci.org/promoutils/reference/pkg_authors.md)
  : Get package author names
- [`pkgs_ru()`](https://docs.ropensci.org/promoutils/reference/pkgs_ru.md)
  : List of packages and details from R-Universe API
- [`post_time()`](https://docs.ropensci.org/promoutils/reference/post_time.md)
  : Get the next post date/time
- [`prs_list()`](https://docs.ropensci.org/promoutils/reference/prs_list.md)
  : List PRs
- [`replace_emoji()`](https://docs.ropensci.org/promoutils/reference/replace_emoji.md)
  : Replace emoji codes with unicode
- [`socials_post_issue()`](https://docs.ropensci.org/promoutils/reference/socials_post_issue.md)
  : Create a draft issue to post to Mastodon and LinkedIn
- [`url_from_path()`](https://docs.ropensci.org/promoutils/reference/url_from_path.md)
  : Create url from content date and slug
- [`url_from_api()`](https://docs.ropensci.org/promoutils/reference/url_from_api.md)
  : Convert an api url to a user-facing url
- [`yaml_extract()`](https://docs.ropensci.org/promoutils/reference/yaml_extract.md)
  : Extract YAML keys from block
