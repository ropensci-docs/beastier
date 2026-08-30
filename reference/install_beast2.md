# Deprecated function to install BEAST2

This function is deprecated as it violated CRAN policy.

## Usage

``` r
install_beast2(
  folder_name = rappdirs::user_data_dir(),
  beast2_version = beastier::get_default_beast2_version(),
  verbose = FALSE,
  os = rappdirs::app_dir()$os
)
```

## Arguments

- folder_name:

  name of the folder where the BEAST2 files will be put. The name of the
  BEAST2 binary file will be at `[folder_name]/beast/bin/beast` The name
  of the BEAST2 jar file will be at
  `[folder_name]/beast/lib/launcher.jar`

- beast2_version:

  the version of BEAST2. By default, this is the version as returned by
  [get_default_beast2_version](https://docs.ropensci.org/beastier/reference/get_default_beast2_version.md)

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

Nothing. Gives a deprecation message using
[stop](https://rdrr.io/r/base/stop.html).

## Details

To install BEAST2 from R, go to
<https://github.com/richelbilderbeek/beastierinstall>.

## Author

Richèl J.C. Bilderbeek
