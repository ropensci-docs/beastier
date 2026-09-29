# Check if the input is a valid number of threads.

Will [stop](https://rdrr.io/r/base/stop.html) if not.

## Usage

``` r
check_n_threads(n_threads)
```

## Arguments

- n_threads:

  the number of computational threads to use. Use
  [NA](https://rdrr.io/r/base/NA.html) to use the BEAST2 default of 1.

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if the number of
threads in invalid

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

# Can have 1 or more threads
check_n_threads(1)
check_n_threads(2)
# Can have NA threads
check_n_threads(NA)
#> NULL

check_empty_beaustier_folders()
```
