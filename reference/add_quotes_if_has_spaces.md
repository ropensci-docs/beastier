# Add quotes around the string if it contains spaces.

Add quotes around the string if it contains spaces. Does nothing if the
string contains no spaces. This is used for filenames

## Usage

``` r
add_quotes_if_has_spaces(filename)
```

## Arguments

- filename:

  a filename

## Value

a filename. If the filename did not contain spaces, it is returned
as-is. If the filename did contain spaces, the filename is surrounded by
quotes

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
remove_beaustier_folders()
check_empty_beaustier_folders()

add_quotes_if_has_spaces("x")
#> [1] "x"
add_quotes_if_has_spaces("a b")
#> [1] "'a b'"

check_empty_beaustier_folders()
```
