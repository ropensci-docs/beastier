# Check if the `beast2_options` is a valid BEAST2 options object.

Calls `stop` if the BEAST2 option object is invalid

## Usage

``` r
check_beast2_optionses(beast2_optionses)
```

## Arguments

- beast2_optionses:

  list of one or more `beast2_options` structures, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md).
  Use of reduplicated plural to achieve difference with `beast2_options`

## Value

Nothing. Will `stop` if the BEAST2 option object is invalid

## See also

Use
[create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)
to create a valid BEAST2 options object

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

check_beast2_optionses(list(create_beast2_options()))

check_empty_beaustier_folders()
```
