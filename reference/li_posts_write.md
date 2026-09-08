# Post to LinkedIn

Post to LinkedIn

## Usage

``` r
li_posts_write(author, body, dry_run = FALSE)
```

## Arguments

- author:

  Character. URN. Either yours (see
  [`li_urn_me()`](https://docs.ropensci.org/promoutils/reference/li_urn_me.md)
  or rOpenSci's "urn:li:organization:77132573")

- body:

  Character. The body of the post as you would like it to appear.

- dry_run:

  Logical. TRUE to show what would be sent to the server without
  actually sending it.

## Value

A string of the URN for the post id.

## Examples

``` r
# Dry-run
id <- li_posts_write(
  author = ro_urn, # Post on behalf of rOpenSci
  body = "Testing out the LinkedIn API via R and httr2!",
  dry_run = TRUE)
#> POST /rest/posts HTTP/1.1
#> accept: */*
#> accept-encoding: deflate, gzip, br, zstd
#> content-length: 291
#> content-type: application/json
#> host: api.linkedin.com
#> linkedin-version: 202510
#> user-agent: httr2/1.3.0 r-curl/8.0.0 libcurl/8.5.0
#> x-restli-protocol-version: 2.0.0
#> 
#> {
#>   "author": "urn:li:organization:77132573",
#>   "commentary": "Testing out the LinkedIn API via R and httr2!",
#>   "visibility": "PUBLIC",
#>   "distribution": {
#>     "feedDistribution": "MAIN_FEED",
#>     "targetEntities": [
#> 
#>     ],
#>     "thirdPartyDistributionChannels": [
#> 
#>     ]
#>   },
#>   "lifecycleState": "PUBLISHED",
#>   "isReshareDisabledByAuthor": false
#> }

if (FALSE) { # \dontrun{
# Real post
id <- li_posts_write(
  author = ro_urn, # Post on behalf of rOpenSci
  body = "Testing out the LinkedIn API via R and httr2!")
} # }
```
