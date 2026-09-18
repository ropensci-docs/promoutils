# Replace emoji codes with unicode

Replaces emoji codes like :tada: with unicode like 🎉.

## Usage

``` r
replace_emoji(x)
```

## Arguments

- x:

  Character. Text string within which to replace codes

## Value

Text string with emoji unicodes

## Examples

``` r
replace_emoji("hi :tada: testing \n\n\n Whow ! 🔗 \n\n\n :smile:")
#> [1] "hi 🎉 testing \n\n\n Whow ! 🔗 \n\n\n 😄"
replace_emoji(":link:")
#> [1] "🔗"
```
