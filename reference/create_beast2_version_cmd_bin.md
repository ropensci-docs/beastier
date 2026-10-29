# Creates the terminal command to version a BEAST2 input file using a call to the `launcher.jar` file

Creates the terminal command to version a BEAST2 input file using a call
to the `launcher.jar` file

## Usage

``` r
create_beast2_version_cmd_bin(
  beast2_bin_path = beastier::get_default_beast2_bin_path()
)
```

## Arguments

- beast2_bin_path:

  name of the BEAST2 binary file (usually simply `beast`). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path

## Value

a character vector, of which the first element is the command (`java`,
in this case), and the others are arguments (`-jar`, in this case,
followed by more arguments.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
  if (is_beast2_installed() && beautier::is_on_ci()) {
    create_beast2_version_cmd_bin()
  }
```
