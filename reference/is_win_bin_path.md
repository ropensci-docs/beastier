# Is the path a path to the BEAST2 binary file? Does not check if the file at that path is present

Is the path a path to the BEAST2 binary file? Does not check if the file
at that path is present

## Usage

``` r
is_win_bin_path(path)
```

## Arguments

- path:

  a string to a path

## Value

TRUE if the path is a path to a BEAST2 binary file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

# TRUE
is_win_bin_path("BEAST.exe")
#> [1] TRUE
# FALSE
is_win_bin_path("beast")
#> [1] FALSE
is_win_bin_path("launcher.jar")
#> [1] FALSE

check_empty_beaustier_folders()
```
