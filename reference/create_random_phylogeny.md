# Create a random phylogeny

Create a random phylogeny

## Usage

``` r
create_random_phylogeny(n_taxa, taxa_name_ext = "")
```

## Arguments

- n_taxa:

  The number of taxa

- taxa_name_ext:

  the extension of the taxa names

## Value

a phylogeny of class \`phylo\` (which is part of the \`ape\` package)

## Author

Richèl J.C. Bilderbeek

## Examples

``` r
create_random_phylogeny(n_taxa = 6)
#> 
#> Phylogenetic tree with 6 tips and 5 internal nodes.
#> 
#> Tip labels:
#>   t5, t3, t4, t1, t6, t2
#> 
#> Rooted; includes branch length(s).
```
