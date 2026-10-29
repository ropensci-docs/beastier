# Deprecated function to uninstall BEAST2

Deprecated function to uninstall BEAST2

## Usage

``` r
uninstall_beast2(
  folder_name = rappdirs::user_data_dir(),
  os = rappdirs::app_dir()$os,
  verbose = FALSE
)
```

## Arguments

- folder_name:

  name of the folder where the BEAST2 files are installed. The name of
  the BEAST2 binary file will be at `[folder_name]/beast/bin/beast` The
  name of the BEAST2 jar file will be at
  `[folder_name]/beast/lib/launcher.jar`

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

## Value

Nothing. A deprecation message using
[stop](https://rdrr.io/r/base/stop.html) will be triggered

## Author

Richèl J.C. Bilderbeek
