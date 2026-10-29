# Get the alignment ID from a file with one alignment

Get the alignment ID from a file with one alignment

## Usage

``` r
get_alignment_ids_from_xml_filename(xml_filename)
```

## Arguments

- xml_filename:

  name of a BEAST2 XML input filename

## Value

one or more alignment IDs

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

# test_output_0
get_alignment_ids_from_xml_filename(get_beastier_path("2_4.xml"))
#> [1] "test_output_0"
# c("anthus_aco","anthus_nd2")
get_alignment_ids_from_xml_filename(get_beastier_path("anthus_15_15.xml"))
#> [1] "anthus_aco" "anthus_nd2"

check_empty_beaustier_folders()
```
