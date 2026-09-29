# Create a random alignment

Create a random alignment

## Usage

``` r
create_random_alignment(n_taxa, sequence_length, rate = 1, taxa_name_ext = "")
```

## Arguments

- n_taxa:

  The number of taxa

- sequence_length:

  The number of base pairs the alignment will have

- rate:

  mutation rate

- taxa_name_ext:

  the extension of the taxa names

## Value

an alignment of class [DNAbin](https://rdrr.io/pkg/ape/man/DNAbin.html)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
check_empty_beaustier_folders()

alignment <- create_random_alignment(
  n_taxa = 5,
  sequence_length = 10
)
image(alignment)


remove_beaustier_folders()
check_empty_beaustier_folders()
```
