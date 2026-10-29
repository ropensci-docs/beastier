# Internal function to extract the screenlog filename for a BEAST2 input file

Extract the screenlog filename from a BEAST2 input file

## Usage

``` r
extract_screenlog_filename_from_beast2_input_file(input_filename)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

## Value

the screenlog filename for a BEAST2 input file

## Author

Richèl J.C. Bilderbeek
