# Checks the BEAST2 `.jar` path. Will stop if there is a problem with the BEAST2 `.jar` path.

Checks the BEAST2 `.jar` path. Will stop if there is a problem with the
BEAST2 `.jar` path.

## Usage

``` r
check_beast2_path(beast2_path)
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

nothing. Will call [`stop`](https://rdrr.io/r/base/stop.html) if the
BEAST2 `.jar` path has a problem

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed()) {
  beast2_path <- get_default_beast2_jar_path()
  check_beast2_path(beast2_path)
}

check_empty_beaustier_folders()
```
