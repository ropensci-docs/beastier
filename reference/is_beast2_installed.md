# Checks if BEAST2 is installed

Checks if BEAST2 is installed

## Usage

``` r
is_beast2_installed(
  folder_name = beastier::get_default_beast2_folder(),
  os = rappdirs::app_dir()$os
)
```

## Arguments

- folder_name:

  name of the folder where the BEAST2 files are put. The name of the
  BEAST2 binary file will be at `[folder_name]/beast/bin/beast` The name
  of the BEAST2 jar file will be at
  `[folder_name]/beast/lib/launcher.jar`

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

TRUE if BEAST2 is installed

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

is_beast2_installed()
#> [1] FALSE

check_empty_beaustier_folders()
```
