# Would these lines of text, when written to a file, result in a valid BEAST2 input file?

Would these lines of text, when written to a file, result in a valid
BEAST2 input file?

## Usage

``` r
are_beast2_input_lines(
  lines,
  verbose = FALSE,
  method = ifelse(beautier::is_on_ci(), "deep", "fast"),
  beast2_path = beastier::get_default_beast2_path()
)
```

## Arguments

- lines:

  lines of text

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

- method:

  the method to check. Can be 'deep' or 'fast'. The 'deep' method uses
  BEAST2 to validate the complete file. The 'fast' method uses some
  superficial tests (for example: if all IDs are unique)

- beast2_path:

  name of either a BEAST2 binary file (usually simply `beast`) or a
  BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

## Value

TRUE if the text is valid, FALSE if not

## See also

Use
[`is_beast2_input_file`](https://docs.ropensci.org/beastier/reference/is_beast2_input_file.md)
to check a file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed() && beautier::is_on_ci()) {
  are_beast2_input_lines(get_beastier_path("anthus_2_4.xml"))

  remove_beaustier_folders()
}
check_empty_beaustier_folders()
```
