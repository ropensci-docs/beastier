# Pretty-print a \`beast2_options\`

Pretty-print a \`beast2_options\`

## Usage

``` r
print_beast2_options(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

Nothing. Will display the \`beast2_options\` using
[cat](https://rdrr.io/r/base/cat.html).

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

print_beast2_options(create_beast2_options())
#> |parameter             |value                                                     |
#> |:---------------------|:---------------------------------------------------------|
#> |input_filename        |/github/home/.cache/beastier/beast2_70e1e9001f6.xml       |
#> |output_state_filename |/github/home/.cache/beastier/beast2_70e5ae71bc4.xml.state |
#> |rng_seed              |NA                                                        |
#> |n_threads             |NA                                                        |
#> |use_beagle            |FALSE                                                     |
#> |overwrite             |TRUE                                                      |
#> |beast2_path           |/github/home/.local/share/beast/lib/launcher.jar          |
#> |verbose               |FALSE                                                     |

check_empty_beaustier_folders()
```
