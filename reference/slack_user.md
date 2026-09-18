# Fetch details on a specific user

Fetch details on a specific user

## Usage

``` r
slack_user(name, users = NULL)
```

## Arguments

- name:

  Character. String to match real name to

- users:

  Data frame. Data frame of users from
  [`slack_users()`](https://docs.ropensci.org/promoutils/reference/slack_users.md).

## Value

Data frame

## Examples

``` r
if (FALSE) { # interactive()
slack_user("Steffi")
}
```
