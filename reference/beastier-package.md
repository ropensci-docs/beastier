# `beastier`: A package to call BEAST2.

`beastier` allows to call BEAST2, a popular Bayesian phylogenetics tool,
using an R interface. 'beastier' closely follows the interface of
BEAST2, including its default settings.

## See also

These are packages associated with `beastier`:

- The package `beautier` can create BEAST2 input files from R

- The package `tracerer` can parse BEAST2 output files from R

- The package `babette` combines the functionality of `beautier`,
  `beastier` and `tracerer` into a single workflow

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

beast2_options <- create_beast2_options(
  input_filename = get_beastier_path("2_4.xml")
)

if (is_beast2_installed() && beautier::is_on_ci()) {
  run_beast2_from_options(beast2_options)
  file.remove(beast2_options$output_state_filename)
  remove_beaustier_folders()
}
```
