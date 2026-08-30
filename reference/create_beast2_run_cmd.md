# Creates the terminal command to run BEAST2

Creates the terminal command to run BEAST2

## Usage

``` r
create_beast2_run_cmd(
  input_filename,
  output_state_filename,
  rng_seed = NA,
  n_threads = NA,
  use_beagle = FALSE,
  overwrite = FALSE,
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

  name of the BEAST2 output file that stores the state (usually has a
  `.xml.state` extension)

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

a character vector with the command and arguments to call BEAST2

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

if (is_beast2_installed()) {
  create_beast2_run_cmd(
    input_filename = "input.xml",
    output_state_filename = "output.xml.state",
    beast2_path = get_default_beast2_jar_path()
  )
}

check_empty_beaustier_folders()
```
