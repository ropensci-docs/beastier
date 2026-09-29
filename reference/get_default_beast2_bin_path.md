# Get the default BEAST2 binary file (`beast`, that is) path

Get the default BEAST2 binary file (`beast`, that is) path

## Usage

``` r
get_default_beast2_bin_path(
  beast2_folder = beastier::get_default_beast2_folder(),
  os = rappdirs::app_dir()$os
)
```

## Arguments

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
  to get the default BEAST2 folder. Use get_default_beast2_bin_path to
  get the full path to the default BEAST2 executable.

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

the default BEAST2 binary file's path

## See also

Use
[get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
to get the default folder in which BEAST2 is installed. Use
[install_beast2](https://docs.ropensci.org/beastier/reference/install_beast2.md)
with default arguments to install BEAST2 to this location.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed()) {
  get_default_beast2_bin_path()
}

check_empty_beaustier_folders()
```
