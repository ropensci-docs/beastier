# Internal function to check if the MCMC's tracelog file can be created.

Check if the MCMC's tracelog file can be created. Will
[stop](https://rdrr.io/r/base/stop.html) if not. If the tracelog file
already exists, it is assumed that a new file can be created, by
overwriting the existing one.

## Usage

``` r
check_can_create_tracelog_file(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if the MCMC's
tracelog file is absent and cannot be created.

## Author

Richèl J.C. Bilderbeek
