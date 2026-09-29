# Get a temporary filename

Get a temporary filename, similar to
[tempfile](https://rdrr.io/r/base/tempfile.html), except that it always
writes to a temporary folder named
[beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md).

## Usage

``` r
get_beastier_tempfilename(pattern = "file", fileext = "")
```

## Arguments

- pattern:

  a non-empty character vector giving the initial part of the name.

- fileext:

  a non-empty character vector giving the file extension

## Value

name for a temporary file

## Note

this function is added to make sure no temporary cache files are left
undeleted

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
get_beastier_tempfilename()
#> [1] "/github/home/.cache/beastier/file735aad1ee7"
get_beastier_tempfilename(pattern = "my_pattern_")
#> [1] "/github/home/.cache/beastier/my_pattern_7355c2af6f5"
get_beastier_tempfilename(fileext = ".ext")
#> [1] "/github/home/.cache/beastier/file7356f7e4adb.ext"
```
