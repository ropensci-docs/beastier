# Checks the input filename. Will stop if there is a problem with the input filename.

Checks the input filename. Will stop if there is a problem with the
input filename.

## Usage

``` r
check_input_filename_validity(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

nothing. Will call [`stop`](https://rdrr.io/r/base/stop.html) if the
input file is invalid

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed()) {
  check_input_filename_validity(
    create_beast2_options(
      input_filename = get_beastier_path("2_4.xml")
    )
  )
}
check_empty_beaustier_folders()
```
