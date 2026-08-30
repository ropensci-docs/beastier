# Get a list with the full paths of all BEAST2 example filenames

Get a list with the full paths of all BEAST2 example filenames

## Usage

``` r
get_beast2_example_filenames(
  beast2_folder = beastier::get_default_beast2_folder()
)
```

## Arguments

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the full path to the default BEAST2 executable.

## Value

a list with the full paths of all BEAST2 example filenames

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed()) {
  get_beast2_example_filenames()
}
```
