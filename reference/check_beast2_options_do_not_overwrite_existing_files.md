# Internal function

Check if the `beast2_options` will not overwrite existing files, when
the 'overwrite' options is set to `FALSE`.

## Usage

``` r
check_beast2_options_do_not_overwrite_existing_files(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if a file is
threatened to be overwritten

## Details

Will [stop](https://rdrr.io/r/base/stop.html) if a file is threatened to
be overwritten

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

check_beast2_options_do_not_overwrite_existing_files(
  beast2_options = create_beast2_options()
)

check_empty_beaustier_folders()
```
