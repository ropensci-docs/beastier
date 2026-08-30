# Convert a `beast2_options` to a table

Convert a `beast2_options` to a table

## Usage

``` r
beast2_options_to_table(beast2_options)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

## Value

a [tibble](https://tibble.tidyverse.org/reference/tibble.html) with two
columns, called \`parameter\` and \`value\`. Each \`parameter\` is the
name of the element of the \`beast2_options\` structure, where the
\`value\` on the same row holds the value of that parameter

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
beast2_options_to_table(create_beast2_options())
#> # A tibble: 8 × 2
#>   parameter             value                                                   
#>   <chr>                 <chr>                                                   
#> 1 input_filename        /github/home/.cache/beastier/beast2_70e744c5729.xml     
#> 2 output_state_filename /github/home/.cache/beastier/beast2_70e553bd098.xml.sta…
#> 3 rng_seed              NA                                                      
#> 4 n_threads             NA                                                      
#> 5 use_beagle            FALSE                                                   
#> 6 overwrite             TRUE                                                    
#> 7 beast2_path           /github/home/.local/share/beast/lib/launcher.jar        
#> 8 verbose               FALSE                                                   
```
