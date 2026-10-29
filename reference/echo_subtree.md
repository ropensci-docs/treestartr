# Print subtrees with tips added.

Once a tip has been added to the tree, print the newick-formatted
subtree to which the tip was added.

## Usage

``` r
echo_subtree(tree, mrca_list, tip)
```

## Arguments

- tree:

  Tree to which the tip will be added; object of type phylo

- mrca_list:

  Vector of taxa. The added tip will subtend the MRCA of these taxa

- tip:

  Taxon which will be added to the tree.

## Value

tree subtree to which tip was added

## Examples

``` r
mrca_list <- c("Ursus_arctos", "Ursus_spelaeus", "Ursus_americanus")
tree <- text_placr(tree, mrca_df)
#> Placing tip Kretzoiarctos_beatrix
#> via relatives Indarctos_arctoides, Indarctos_vireti
#>  at node 25
#> Placing tip Ursus_abstrusus
#> via relatives Ursus_arctos, Ursus_spelaeus, Ursus_americanus
#>  at node 30
echo_sub <- echo_subtree(tree, mrca_list, "Ursus_abstrusus")
```
