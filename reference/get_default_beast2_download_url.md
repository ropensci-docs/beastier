# Get the default BEAST2 download URL, which depends on the operating system

Get the default BEAST2 download URL, which depends on the operating
system

## Usage

``` r
get_default_beast2_download_url(
  beast2_version = beastier::get_default_beast2_version(),
  os = rappdirs::app_dir()$os
)
```

## Arguments

- beast2_version:

  the version of BEAST2. By default, this is the version as returned by
  [get_default_beast2_version](https://docs.ropensci.org/beastier/reference/get_default_beast2_version.md)

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

## Value

the URL where BEAST2 can be downloaded from

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
get_default_beast2_download_url()
#> [1] "https://github.com/CompEvol/beast2/releases/download/v2.6.0/BEAST.v2.6.0.Linux.tgz"
```
