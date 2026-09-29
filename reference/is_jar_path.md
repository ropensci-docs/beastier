# Is the path a path to the BEAST2 jar file? Does not check if the file at that path is present

Is the path a path to the BEAST2 jar file? Does not check if the file at
that path is present

## Usage

``` r
is_jar_path(path)
```

## Arguments

- path:

  a string to a path

## Value

TRUE if the path is a path to a BEAST2 jar file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
# Returns TRUE
is_jar_path("beast.jar")
#> [1] TRUE
is_jar_path("launcher.jar")
#> [1] TRUE
is_jar_path(get_default_beast2_jar_path())
#> [1] TRUE
# Returns FALSE
is_jar_path("beast")
#> [1] FALSE
is_jar_path(get_default_beast2_bin_path())
#> [1] FALSE
```
