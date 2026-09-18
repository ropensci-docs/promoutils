# Authorize rOpenSci client with LinkedIn

This authorizes the rOpenSci client with **your** credentials (and you
must be part of the rOpenSci organization as an admin). Make sure to
take note of the 'refresh_token' as that is what you'll add to your
.Renviron file for local work, or the GitHub secrets for the
comms/scheduled_socials workflow.

## Usage

``` r
li_auth()
```

## Value

httr2 authorization

## Details

This function authorizes with a redirect url of
"http://localhost:1444/", this *must* be the same as that listed in the
LinkedIn Developer App, https://www.linkedin.com/developers/apps.

**If you retrieve a new token, you will have to put it in the .Renviron
and the re-start your R session to continue**

This function authorizes with the scopes:

- w_member_social (default)

- w_organization_social (special request)

- r_organization_social (special request)

- r_organization_admin (special request)

## References

- Refresh tokens API:
  https://learn.microsoft.com/en-us/linkedin/shared/authentication/programmatic-refresh-tokens

## Examples

``` r
if (FALSE) { # \dontrun{
# Only run if you need to update the scopes or get a new token (otherwise
# you'll have to replace all your tokens)
t <- li_auth()
t$refresh_token
} # }
```
