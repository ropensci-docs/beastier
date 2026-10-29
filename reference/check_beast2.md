# Check if `BEAST2` is installed properly.

Calls [stop](https://rdrr.io/r/base/stop.html) if BEAST2 is improperly
installed

## Usage

``` r
check_beast2(beast2_path = beastier::get_default_beast2_path())
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

nothing Will [stop](https://rdrr.io/r/base/stop.html) if BEAST2 is
improperly installed

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed()) {
  check_beast2()
}
```
