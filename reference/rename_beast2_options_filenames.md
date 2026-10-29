# Rename the filenames in the BEAST2 options

Rename the filenames in the BEAST2 options

## Usage

``` r
rename_beast2_options_filenames(beast2_options, rename_fun)
```

## Arguments

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

- rename_fun:

  a function to rename a filename, as can be checked by
  [check_rename_fun](https://docs.ropensci.org/beautier/reference/check_rename_fun.html).
  This function should have one argument, which will be a filename or
  [NA](https://rdrr.io/r/base/NA.html). The function should
  [return](https://rdrr.io/r/base/function.html) one filename (when
  passed one filename) or one [NA](https://rdrr.io/r/base/NA.html) (when
  passed one [NA](https://rdrr.io/r/base/NA.html)). Example rename
  functions are:

  - [get_remove_dir_fun](https://docs.ropensci.org/beautier/reference/get_remove_dir_fun.html)
    get a function that removes the directory paths from the filenames,
    in effect turning these into local files

  - [get_replace_dir_fun](https://docs.ropensci.org/beautier/reference/get_replace_dir_fun.html)
    get a function that replaces the directory paths from the filenames

  - [get_remove_hex_fun](https://docs.ropensci.org/beautier/reference/get_remove_hex_fun.html)
    get a function that removes the hex string from filenames. For
    example, `tracelog_82c1a522040.log` becomes `tracelog.log`

## Value

a \`beast2_options\` with the filenames it contains renamed

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

# beast2_options with local filenames
beast2_options <- create_beast2_options(
  input_filename = "my.fas",
  output_state_filename = "my_state.xml.state"
)
# Rename filenames to be in /my/new/folder
rename_beast2_options_filenames(
  beast2_options = beast2_options,
  rename_fun = beautier::get_replace_dir_fun("/my/new/folder")
)
#> $input_filename
#> [1] "/my/new/folder/my.fas"
#> 
#> $output_state_filename
#> [1] "/my/new/folder/my_state.xml.state"
#> 
#> $rng_seed
#> [1] NA
#> 
#> $n_threads
#> [1] NA
#> 
#> $use_beagle
#> [1] FALSE
#> 
#> $overwrite
#> [1] TRUE
#> 
#> $beast2_path
#> [1] "/github/home/.local/share/beast/lib/launcher.jar"
#> 
#> $verbose
#> [1] FALSE
#> 

check_empty_beaustier_folders()
```
