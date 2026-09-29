# Get the .trees filenames that BEAST2 will produce

Get the .trees filenames that BEAST2 will produce

## Usage

``` r
get_trees_filenames(input_filename)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

## Value

character vector with the names of the .trees files that BEAST2 will
produce

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

get_trees_filenames(get_beastier_path("2_4.xml"))
#> [1] "test_output_0.trees"
get_trees_filenames(get_beastier_path("anthus_2_4.xml"))
#> [1] "Anthus_nd2.trees" "Anthus_aco.trees"

check_empty_beaustier_folders()
```
