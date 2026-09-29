# Get the full path of a file in the `inst/extdata` folder

Get the full path of a file in the `inst/extdata` folder

## Usage

``` r
get_beastier_path(filename)
```

## Arguments

- filename:

  the file's name, without the path

## Value

the full path to the filename. Will `stop` if the file is absent in the
`inst/extdata` folder

## See also

for more files, use
[`get_beastier_paths`](https://docs.ropensci.org/beastier/reference/get_beastier_paths.md)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
get_beastier_path("beast2_example_output.log")
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/beastier/extdata/beast2_example_output.log"
get_beastier_path("beast2_example_output.trees")
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/beastier/extdata/beast2_example_output.trees"
get_beastier_path("beast2_example_output.xml")
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/beastier/extdata/beast2_example_output.xml"
get_beastier_path("beast2_example_output.xml.state")
#> [1] "/github/home/R/x86_64-pc-linux-gnu-library/4.6/beastier/extdata/beast2_example_output.xml.state"
```
