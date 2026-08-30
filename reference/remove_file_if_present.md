# Remove a file if it is present, will do nothing if it is not.

Remove a file if it is present, will do nothing if it is not.

## Usage

``` r
remove_file_if_present(filename)
```

## Arguments

- filename:

  name of a file

## Value

Nothing. Will remove the file if it is presented, will do nothing if it
is not.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
filename <- tempfile()
file.create(filename)
#> [1] TRUE
remove_file_if_present(filename)
#> [1] TRUE
remove_file_if_present(filename)
```
