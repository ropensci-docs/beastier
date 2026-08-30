# Get the path to the folder where this package installs BEAST2 by default

Get the path to the folder where this package installs BEAST2 by default

## Usage

``` r
get_default_beast2_folder()
```

## Value

the path to the folder where this package installs BEAST2 by default

## See also

Use
[get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
to get the path to the BEAST2 jar file, when installed by this package
Use
[install_beast2](https://docs.ropensci.org/beastier/reference/install_beast2.md)
with default arguments to install BEAST2 to this folder.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

get_default_beast2_folder()
#> [1] "~/.local/share"

check_empty_beaustier_folders()
```
