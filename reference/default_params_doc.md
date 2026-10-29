# This function does nothing. It is intended to inherit is parameters' documentation.

This function does nothing. It is intended to inherit is parameters'
documentation.

## Usage

``` r
default_params_doc(
  beast2_bin_path,
  beast2_folder,
  beast2_jar_path,
  beast2_options,
  beast2_optionses,
  beast2_path,
  beast2_version,
  beast2_working_dir,
  beastier_folder,
  beautier_folder,
  clock_model,
  clock_models,
  crown_age,
  crown_ages,
  fasta_filename,
  fasta_filenames,
  fixed_crown_age,
  fixed_crown_ages,
  initial_phylogenies,
  input_filename,
  mcmc,
  misc_options,
  n_taxa,
  n_threads,
  os,
  output_filename,
  output_log_filename,
  output_state_filename,
  output_trees_filenames,
  overwrite,
  rename_fun,
  rng_seed,
  sequence_length,
  site_model,
  site_models,
  tree_prior,
  tree_priors,
  use_beagle,
  verbose
)
```

## Arguments

- beast2_bin_path:

  name of the BEAST2 binary file (usually simply `beast`). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path

- beast2_folder:

  the folder where the BEAST2 is installed. Note that this is not the
  folder where the BEAST2 executable is installed: the BEAST2 executable
  is in a subfolder. Use
  [get_default_beast2_folder](https://docs.ropensci.org/beastier/reference/get_default_beast2_folder.md)
  to get the default BEAST2 folder. Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the full path to the default BEAST2 executable.

- beast2_jar_path:

  name of the BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

- beast2_options:

  a set of BEAST2 options, that are the R equivalent of the BEAST2
  command-line options, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md)

- beast2_optionses:

  list of one or more `beast2_options` structures, as can be created by
  [create_beast2_options](https://docs.ropensci.org/beastier/reference/create_beast2_options.md).
  Use of reduplicated plural to achieve difference with `beast2_options`

- beast2_path:

  name of either a BEAST2 binary file (usually simply `beast`) or a
  BEAST2 jar file (usually has a `.jar` extension). Use
  [get_default_beast2_bin_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_bin_path.md)
  to get the default BEAST binary file's path Use
  [get_default_beast2_jar_path](https://docs.ropensci.org/beastier/reference/get_default_beast2_jar_path.md)
  to get the default BEAST jar file's path

- beast2_version:

  the version of BEAST2. By default, this is the version as returned by
  [get_default_beast2_version](https://docs.ropensci.org/beastier/reference/get_default_beast2_version.md)

- beast2_working_dir:

  a folder where BEAST2 can work in isolation. For each BEAST2 run, a
  new subfolder is created in that folder. Within this folder, BEAST2 is
  allowed to create all of its output files, without the risk of
  overwriting existing ones, allowing BEAST2 to run in multiple parallel
  processes.

- beastier_folder:

  the path to the
  [beastier](https://docs.ropensci.org/beastier/reference/beastier-package.md)
  temporary files folder

- beautier_folder:

  temporary folder used by
  [beautier](https://docs.ropensci.org/beautier/reference/beautier-package.html)

- clock_model:

  a `beautier` clock model

- clock_models:

  a list of one or more `beautier` clock models

- crown_age:

  the crown age of the phylogeny

- crown_ages:

  the crown ages of the phylogenies. Set to NA if the crown age needs to
  be estimated

- fasta_filename:

  a FASTA filename.

- fasta_filenames:

  One or more FASTA filenames.

- fixed_crown_age:

  determines if the phylogeny's crown age is fixed. If FALSE, crown age
  is estimated by BEAST2. If TRUE, the crown age is fixed to the crown
  age of the initial phylogeny.

- fixed_crown_ages:

  one or more booleans to determine if the phylogenies' crown ages are
  fixed. If FALSE, crown age is estimated by BEAST2. If TRUE, the crown
  age is fixed to the crown age of the initial phylogeny.

- initial_phylogenies:

  one or more MCMC chain's initial phylogenies. Each one set to NA will
  result in BEAST2 using a random phylogeny. Else the phylogeny is
  assumed to be of class
  [`ape::phylo`](https://rdrr.io/pkg/ape/man/read.tree.html).

- input_filename:

  the name of a BEAST2 input XML file. This file usually has an `.xml`
  extension. Use
  [create_temp_input_filename](https://docs.ropensci.org/beastier/reference/create_temp_input_filename.md)
  to create a temporary filename with that extension.

- mcmc:

  one `beautier` MCMC

- misc_options:

  one `beautier` misc_options object

- n_taxa:

  The number of taxa

- n_threads:

  the number of computational threads to use. Use
  [NA](https://rdrr.io/r/base/NA.html) to use the BEAST2 default of 1.

- os:

  name of the operating system, must be `unix` (Linux, Mac) or `win`
  (Windows)

- output_filename:

  Name of the XML parameter file created by this function. BEAST2 uses
  this file as input.

- output_log_filename:

  name of the .log file to create

- output_state_filename:

  name of the `.xml.state` file to create. Use
  [create_temp_state_filename](https://docs.ropensci.org/beastier/reference/create_temp_state_filename.md)
  to create a temporary filename with that extension.

- output_trees_filenames:

  one or more names for .trees file to create. There will be one .trees
  file created per alignment in the input file. The number of alignments
  must equal the number of .trees filenames, else an error is thrown.
  Alignments are sorted alphabetically by their IDs

- overwrite:

  if TRUE: overwrite the `.log` and `.trees` files if one of these
  exists. If FALSE, BEAST2 will not be started if

  - the `.log` file exists

  - the `.trees` files exist

  - the `.log` file created by BEAST2 exists

  - the `.trees` files created by BEAST2 exist

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

- rng_seed:

  the random number generator seed of the BEAST2 run. Must be a non-zero
  positive integer value or [NA](https://rdrr.io/r/base/NA.html). If
  `rng_seed` is [NA](https://rdrr.io/r/base/NA.html), BEAST2 will pick a
  random seed

- sequence_length:

  a DNA sequence length, in base pairs

- site_model:

  a `beautier` site model

- site_models:

  one or more `beautier` site models

- tree_prior:

  a `beautier` tree prior

- tree_priors:

  one or more `beautier` tree priors

- use_beagle:

  use BEAGLE if present

- verbose:

  if TRUE, additional information is displayed, that is potentially
  useful in debugging

## Value

Nothing. This is an internal function that does nothing

## Note

This is an internal function, so it should be marked with `@noRd`. This
is not done, as this will disallow all functions to find the
documentation parameters

## Author

Richèl J.C. Bilderbeek
