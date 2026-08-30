# Create the folder where the BEAST2 state output file will be created

Create the folder where the BEAST2 state output file will be created

## Usage

``` r
create_beast2_state_output_file_folder(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

nothing

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

beast2_options <- create_beast2_options()
create_beast2_state_output_file_folder(beast2_options)

remove_beaustier_folders()
check_empty_beaustier_folders()
```
