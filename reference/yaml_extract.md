# Extract YAML keys from block

Extract YAML keys from block

## Usage

``` r
yaml_extract(yaml, trim = "~~~")
```

## Arguments

- yaml:

  Character. String from which to extract YAML keys

- trim:

  Character. Text to remove from the YAML block before processing.
  Usually the text that defines the block.

## Value

data frame of yaml keys

## Examples

``` r

yaml_extract("~~~start: 2023-11-12\nauthor: Steffi\n~~~")
#>        start author
#> 1 2023-11-12 Steffi
```
