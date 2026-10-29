# Run BEAST2

Run BEAST2

## Usage

``` r
run_beast2(
  input_filename,
  output_state_filename = beastier::create_temp_state_filename(),
  rng_seed = NA,
  n_threads = NA,
  use_beagle = FALSE,
  overwrite = TRUE,
  beast2_path = beastier::get_default_beast2_path(),
  verbose = FALSE
)
```

## Arguments

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

- output_state_filename:

  name of the `.xml.state` file to create. Use
  [create_temp_state_filename](https://docs.ropensci.org/beastier/reference/create_temp_state_filename.md)
  to create a temporary filename with that extension.

- rng_seed:

  the random number generator seed of the BEAST2 run. Must be a non-zero
  positive integer value or [NA](https://rdrr.io/r/base/NA.html). If
  `rng_seed` is [NA](https://rdrr.io/r/base/NA.html), BEAST2 will pick a
  random seed

- n_threads:

  the number of computational threads to use. Use
  [NA](https://rdrr.io/r/base/NA.html) to use the BEAST2 default of 1.

- use_beagle:

  use BEAGLE if present

- overwrite:

  if TRUE: overwrite the `.log` and `.trees` files if one of these
  exists. If FALSE, BEAST2 will not be started if

  - the `.log` file exists

  - the `.trees` files exist

  - the `.log` file created by BEAST2 exists

  - the `.trees` files created by BEAST2 exist

- beast2_path:

  name of either a BEAST2 binary file (usually simply `beast`) or a
  BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

## Value

The text sent to `STDOUT` and `STDERR`. It will create the file with
name `output_state_filenames`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed() && beautier::is_on_ci()) {

  output_state_filename <- create_temp_state_filename()

  run_beast2(
    input_filename = get_beastier_path("2_4.xml"),
    output_state_filename = output_state_filename

  )
  file.remove(output_state_filename)
  remove_beaustier_folders()
}

check_empty_beaustier_folders()
```
