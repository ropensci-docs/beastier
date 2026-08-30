# Determines if BEAST2 issues a warning when using the BEAST2 XML input file

Determines if BEAST2 issues a warning when using the BEAST2 XML input
file

## Usage

``` r
gives_beast2_warning(
  filename,
  verbose = FALSE,
  beast2_path = beastier::get_default_beast2_path()
)
```

## Arguments

- filename:

  name of the BEAST2 XML input file

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

TRUE if the file produces a BEAST2 warning, FALSE if not

## See also

Use
[`is_beast2_input_file`](https://docs.ropensci.org/beastier/reference/is_beast2_input_file.md)
to check if a file is a valid BEAST2 input file. Use
[`are_beast2_input_lines`](https://docs.ropensci.org/beastier/reference/are_beast2_input_lines.md)
to check if the text (for example, as loaded from a file) to be valid
BEAST2 input.

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed() &&
  beautier::is_on_ci() &&
  rappdirs::app_dir()$os == "unix") {

  # This file is OK for BEAST2, no warning, returns FALSE
  gives_beast2_warning(filename = get_beastier_path("2_4.xml"))

  # BEAST2 will give a warning on this file, returns TRUE
  gives_beast2_warning(
    filename = get_beastier_path("beast2_warning.xml")
  )
}
```
