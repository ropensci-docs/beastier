# Check if the input is a valid RNG seed.

Will [stop](https://rdrr.io/r/base/stop.html) if not.

## Usage

``` r
check_rng_seed(rng_seed)
```

## Arguments

- rng_seed:

  the random number generator seed of the BEAST2 run. Must be a non-zero
  positive integer value or [NA](https://rdrr.io/r/base/NA.html). If
  `rng_seed` is [NA](https://rdrr.io/r/base/NA.html), BEAST2 will pick a
  random seed

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if the RNG seed
is invalid

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

# Numbers from 1 and higher are valid RNG seeds
check_rng_seed(1)
check_rng_seed(2)
# Also NA is a valid RNG seed
check_rng_seed(NA)
#> NULL

check_empty_beaustier_folders()
```
