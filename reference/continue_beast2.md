# Continue a BEAST2 run

Continue a BEAST2 run

## Usage

``` r
continue_beast2(beast2_options = beastier::create_beast2_options())
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

The text sent to `STDOUT` and `STDERR`. It will create the file with
name `output_state_filenames`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed() && beautier::is_on_ci()) {
  beast2_options <- create_beast2_options(
    input_filename = get_beastier_path("2_4.xml")
  )
  run_beast2_from_options(beast2_options)
  continue_beast2(beast2_options)
  file.remove(beast2_options$output_state_filename)
  remove_beaustier_folders()
}

check_empty_beaustier_folders()
```
