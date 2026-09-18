# Dictionary for usecases

Creates a data frame dictionary of different versions of wording to use
in usecase posts depending on the language of the post.

## Usage

``` r
dict_usecases()
```

## Value

Data frame.

## Examples

``` r
dict_usecases()
#> # A tibble: 2 × 7
#>   category     l_using l_by  l_maintained  l_intro_mult   l_intro_single l_share
#>   <chr>        <chr>   <chr> <chr>         <chr>          <chr>          <chr>  
#> 1 Casos de Uso Usando  por   mantenido por [casos de uso… [casos de uso… ¡Compa…
#> 2 Use Cases    Using   by    maintained by [use cases] N… [use cases] U… Share …
```
