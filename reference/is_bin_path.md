# Is the path a path to the BEAST2 binary file? Does not check if the file at that path is present

Is the path a path to the BEAST2 binary file? Does not check if the file
at that path is present

## Usage

``` r
is_bin_path(path)
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

if (is_beast2_installed()) {
  # TRUE
  is_bin_path("beast")
  is_bin_path("BEAST.exe")
  is_bin_path(get_default_beast2_bin_path())
  # FALSE
  is_bin_path("launcher.jar")
  is_bin_path(get_default_beast2_jar_path())
}

check_empty_beaustier_folders()
```
