# Get the BEAST2 version

Get the BEAST2 version

## Usage

``` r
get_beast2_version(beast2_path = beastier::get_default_beast2_path())
```

## Arguments

- beast2_path:

  name of either a BEAST2 binary file (usually simply `beast`) or a
  BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

## Value

the BEAST2 version

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed() && beautier::is_on_ci()) {
  get_beast2_version()
}

check_empty_beaustier_folders()
```
