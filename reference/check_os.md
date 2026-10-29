# Checks if the operating system is supported

Checks if the operating system is supported

## Usage

``` r
check_os(os)
```

## Arguments

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

Nothing. Will [stop](https://rdrr.io/r/base/stop.html) if the OS is
unsupported

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

check_os("mac")
check_os("unix")
check_os("win")

check_empty_beaustier_folders()
```
