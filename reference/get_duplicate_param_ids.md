# Find duplicate `RealParameter` IDs

Find duplicate `RealParameter` IDs

## Usage

``` r
get_duplicate_param_ids(text)
```

## Arguments

- text:

  the XML as text

## Value

a vector of duplicate IDs, will be empty if all IDs are unique

## See also

to see if all IDs are unique, use
[`has_unique_ids`](https://docs.ropensci.org/beastier/reference/has_unique_ids.md)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

line_1 <- "<parameter id=\"RealParameter.1\" ...</parameter>"
line_2 <- "<parameter id=\"RealParameter.2\" ...</parameter>"
# No elements
get_duplicate_param_ids(c(line_1, line_2))
#> character(0)

# 'RealParameter.1'
get_duplicate_param_ids(c(line_1, line_1))
#> [1] "RealParameter.1"

# 'RealParameter.2'
get_duplicate_param_ids(c(line_2, line_2))
#> [1] "RealParameter.2"

check_empty_beaustier_folders()
```
