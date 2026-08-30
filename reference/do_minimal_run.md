# Do a minimal BEAST2 run

To achieve this,
[run_beast2_from_options](https://docs.ropensci.org/beastier/reference/run_beast2_from_options.md)
is called.

## Usage

``` r
do_minimal_run()
```

## Value

The text sent to `STDOUT` and `STDERR`. It will create the files with
name `output_state_filename`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
if (is_beast2_installed() && beautier::is_on_ci()) {
  do_minimal_run()
}
```
