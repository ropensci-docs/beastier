# Creates the terminal command to validate a BEAST2 input file using a call to the `launcher.jar` file

Creates the terminal command to validate a BEAST2 input file using a
call to the `launcher.jar` file

## Usage

``` r
create_beast2_validate_cmd_jar(
  input_filename,
  beast2_jar_path = beastier::get_default_beast2_jar_path()
)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

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
check_empty_beaustier_folders()

if (is_beast2_installed() && beautier::is_on_ci()) {
  create_beast2_validate_cmd_jar(
    input_filename = "input.xml"
  )
}

check_empty_beaustier_folders()
```
