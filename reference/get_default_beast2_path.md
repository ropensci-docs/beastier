# Get the default BEAST2 path

Get the default BEAST2 path

## Usage

``` r
get_default_beast2_path(
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
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the full path to the default BEAST2 executable.

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

the default BEAST2 path

## See also

Use
[get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
to get the default path to the BEAST2 binary file. Use
[get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
to get the default path to the BEAST2 jar file. Use
[get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
to get the default folder in which BEAST2 is installed. Use
[install_beast2](https://docs.ropensci.org/beastier/reference/install_beast2.md)
with default arguments to install BEAST2 to this location.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed()) {
  get_default_beast2_path()
}
```
