# Creates the terminal command to run BEAST2 from a `beast2_options`

If the BEAST2 input `.xml` filename or the BEAST2 state `.state.xml`
filename contain spaces, these filenames are quoted, so that the
command-line interface to BEAST2 correctly parses its arguments

## Usage

``` r
create_beast2_continue_cmd_from_options(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

a character vector with the command and arguments to call BEAST2

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
  if (is_beast2_installed()) {
    create_beast2_continue_cmd_from_options(
      beast2_options = create_beast2_options()
    )
  }
```
