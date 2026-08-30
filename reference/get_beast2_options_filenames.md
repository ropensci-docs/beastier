# Extract the filenames from a \`beast2_options\`

Extract the filenames from a \`beast2_options\`

## Usage

``` r
get_beast2_options_filenames(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

the filenames from a \`beast2_options\`

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
beast2_options <- create_beast2_options()
get_beast2_options_filenames(beast2_options)
#> [1] "/github/home/.cache/beastier/beast2_70e29d415be.xml"      
#> [2] "/github/home/.cache/beastier/beast2_70e125c80f9.xml.state"
```
