# Add tips to tree via taxon list

Add tips according to csv or tsv file of taxon names and taxa that form
the clade into which you"d like to insert the tip. One column should be
called 'taxon', and should contain the taxon to be placed. The other
column should be called 'clade' and contain the taxon with which the
taxon to be placed will form a group. Each member of the clade will be
placed on its own line. An example of this file can be seen in
\`inst/extdat a/mrca_df.tsv\`

## Usage

``` r
text_placr(tree, mrca_df, echo_subtrees = NULL, echo_revbayes = NULL)
```

## Arguments

- tree:

  Starting tree; object of type phylo

- mrca_df:

  Dataframe containing a column of the taxa you'd like to place and one
  column with the clade into which you'd like to place it

- echo_subtrees:

  Boolean; Print newick subtree with missing taxa added to screen.
  Default FALSE.

- echo_revbayes:

  Boolean; Print clade constraints with missing taxa added to screen,
  formatted for RevBayes fossilized birth-death analysis. Default FALSE.

## Value

tree Phylo object containing the starting tree, and all tips that were
added.

## Examples

``` r
text_placr(tree, mrca_df)
#> Placing tip Kretzoiarctos_beatrix
#> via relatives Indarctos_arctoides, Indarctos_vireti
#>  at node 25
#> Placing tip Ursus_abstrusus
#> via relatives Ursus_arctos, Ursus_spelaeus, Ursus_americanus
#>  at node 30
#> 
#> Phylogenetic tree with 17 tips and 19 internal nodes.
#> 
#> Tip labels:
#>   Ailuropoda_melanoleuca, Agriarctos_spp, Kretzoiarctos_beatrix, Indarctos_arctoides, Indarctos_vireti, Ursus_abstrusus, ...
#> 
#> Rooted; no branch length.
```
