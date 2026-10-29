# Create a random FASTA file

Create a random FASTA file

## Usage

``` r
create_random_fasta(
  n_taxa,
  sequence_length,
  fasta_filename,
  taxa_name_ext = ""
)
```

## Arguments

- n_taxa:

  The number of taxa

- sequence_length:

  a DNA sequence length, in base pairs

- fasta_filename:

  a FASTA filename.

- taxa_name_ext:

  the extension of the taxa names

## Value

Nothing, creates a FASTA file

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

fasta_filename <- get_beastier_tempfilename()
create_random_fasta(
  n_taxa = 5,
  sequence_length = 20,
  fasta_filename = fasta_filename
)
#> NULL
file.remove(fasta_filename)
#> [1] TRUE

remove_beaustier_folders()
check_empty_beaustier_folders()
```
