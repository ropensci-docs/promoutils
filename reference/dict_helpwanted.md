# Dictionary for help-wanted

Creates a data frame dictionary of different versions of wording to use
in help-wanted posts depending on the language of the post.

## Usage

``` r
dict_helpwanted()
```

## Value

Data frame.

## Examples

``` r
dict_helpwanted()
#> # A tibble: 2 × 7
#>   category l_first l_maintainer l_maintained l_intro_mult l_intro_single l_share
#>   <chr>    <chr>   <chr>        <chr>        <chr>        <chr>          <chr>  
#> 1 Se busc… ""      ""           mantenido p… [casos de u… [casos de uso… ¡Compa…
#> 2 Help wa… "A gre… "New Mainta… maintained … [use cases]… [use cases] U… Share …
```
