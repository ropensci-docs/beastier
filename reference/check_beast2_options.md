# Check if the `beast2_options` is a valid BEAST2 options object.

Calls `stop` if the BEAST2 option object is invalid

## Usage

``` r
check_beast2_options(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

nothing Will `stop` if the BEAST2 option object is invalid

## See also

Use
[create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)
to create a valid BEAST2 options object

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

check_beast2_options(create_beast2_options())

check_empty_beaustier_folders()
```
