# Creates the terminal command to version a BEAST2 input file using a call to the `launcher.jar` file

Creates the terminal command to version a BEAST2 input file using a call
to the `launcher.jar` file

## Usage

``` r
create_beast2_version_cmd_jar(
  beast2_jar_path = beastier::get_default_beast2_jar_path()
)
```

## Arguments

- beast2_jar_path:

  name of the BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

## Value

a character vector, of which the first element is the command (`java`,
in this case), and the others are arguments (`-jar`, in this case,
followed by more arguments.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed()) {
  create_beast2_version_cmd_jar()
}
```
