# Is a file a valid BEAST2 input file?

Is a file a valid BEAST2 input file?

## Usage

``` r
is_beast2_input_file(
  filename,
  show_warnings = FALSE,
  verbose = FALSE,
  beast2_path = beastier::get_default_beast2_path()
)
```

## Arguments

- filename:

  name of the BEAST2 XML input file

- show_warnings:

  if TRUE, warnings will shown

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

- beast2_path:

  name of either a BEAST2 binary file (usually simply `beast`) or a
  BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

## Value

TRUE if the file is valid, FALSE if not

## Note

this function only works on standard BEAST2 input files: if a BEAST2
input file is modified to use a certain BEAST2 package, this function
will label it as an invalid file

## See also

Use
[`are_beast2_input_lines`](https://docs.ropensci.org/beastier/reference/are_beast2_input_lines.md)
to check the lines

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed() && beautier::is_on_ci()) {

  filename <- get_beastier_path("anthus_2_4.xml")
  # TRUE, this is a BEAST2 input file
  is_beast2_input_file(filename)

  filename <- get_beastier_path("beast2_example_output.log")
  # FALSE, this is not a BEAST2 input file,
  # it is a BEAST2 output log file insteaf
  is_beast2_input_file(filename)
}

check_empty_beaustier_folders()
```
