# Create Word lists for spelling dictionaries

Creates a word list of packages, and/or maintainer, and/or contributor
names. If wordlist already exists will update existing list.

## Usage

``` r
wordlist_create(
  which = c("packages", "maintainers"),
  path = ".wordlists/names.txt"
)
```

## Arguments

- which:

  Character vector. Which words to create lists for? Any of "packages",
  "maintainers", "contributors".

- path:

  Character. File path to save wordlist to.

## Value

Path of new wordlist

## Examples

``` r
if (FALSE) { # interactive()
wordlist_create()
}
```
