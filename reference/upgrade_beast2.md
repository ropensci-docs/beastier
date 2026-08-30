# Deprecated function to upgrade BEAST2.

Deprecated function to upgrade BEAST2.

## Usage

``` r
upgrade_beast2(
  folder_name = rappdirs::user_data_dir(),
  os = rappdirs::app_dir()$os
)
```

## Arguments

- folder_name:

  name of the folder where the BEAST2 files will be put. The name of the
  BEAST2 binary file will be at `[folder_name]/beast/bin/beast` The name
  of the BEAST2 jar file will be at
  `[folder_name]/beast/lib/launcher.jar`

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

Nothing. A deprecation message using
[stop](https://rdrr.io/r/base/stop.html) will be triggered

## Author

Richèl J.C. Bilderbeek
