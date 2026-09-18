# Get a list of recent posts by rOpenSci

Get a list of recent posts by rOpenSci

## Usage

``` r
li_posts_read(author)
```

## Arguments

- author:

  Character. LinkedIn URN id (e.g., rOpenSci's is
  "urn:li:organization:77132573")

## Value

list of posts

## References

- https://learn.microsoft.com/en-us/linkedin/shared/api-guide/concepts/urns

- https://learn.microsoft.com/en-us/linkedin/marketing/integrations/community-management/shares/posts-api

## Examples

``` r
if (FALSE) { # interactive()
li_posts_read(ro_urn)$elements[[1]]$commentary |> cat()
}
```
