# Determine if the XML text has unique parameter IDs

Determine if the XML text has unique parameter IDs

## Usage

``` r
has_unique_ids(text)
```

## Arguments

- text:

  the XML as text

## Value

TRUE if all parameter IDs are unique, FALSE otherwise

## See also

to obtain the duplicate parameter IDs, use
[`get_duplicate_param_ids`](https://docs.ropensci.org/beastier/reference/get_duplicate_param_ids.md)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

line_1 <- "<parameter id=\"RealParameter.1\" ...</parameter>"
line_2 <- "<parameter id=\"RealParameter.2\" ...</parameter>"
# Unique IDs
has_unique_ids(c(line_1, line_2))
#> [1] TRUE
# No unique ID
has_unique_ids(c(line_1, line_1))
#> [1] FALSE

check_empty_beaustier_folders()
```
