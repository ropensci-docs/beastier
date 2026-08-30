# Checks the input filename. Will stop if there is a problem with the input filename.

Checks the input filename. Will stop if there is a problem with the
input filename.

## Usage

``` r
check_input_filename(input_filename)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if the input file
is invalid

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

check_input_filename(
  get_beastier_path("beast2_example_output.log")
)

check_empty_beaustier_folders()
```
