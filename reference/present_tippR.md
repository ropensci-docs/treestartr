# Add tips to the tree based on taxonomy.

Add tips not on existing tree to the tree via an MRCA node, if they have
congeners. This function will look to see if any tips on the tree have
the same genus as the tip to be added. If there are multiple members of
the genus, the tip will be added subtending the MRCA of all present
congeners. If there is member of the genus, the tip will be added
subtending the parent node of the congener.

## Usage

``` r
present_tippr(tree, absent_list, echo_subtrees = NULL,
  echo_revbayes = NULL)
```

## Arguments

- tree:

  Starting tree; object of type phylo

- absent_list:

  Vector of taxa in the total dataset that are not on the tree

- echo_subtrees:

  Boolean; Print newick subtree with missing taxa added to screen.
  Default FALSE.

- echo_revbayes:

  Boolean; Print clade constraints with missing taxa added to screen,
  formatted for RevBayes fossilized birth-death analysis. Default FALSE.

## Value

tree. Phylo object containing the starting tree, and all tips that were
added.

## Examples

``` r
genera_tree <- present_tippr(tree, absent_list)
#> Tree tip names formatted correctly
#> [1] "Indarctos_arctoides" "Indarctos_vireti"   
#> Warning: 2 arguments not used by format 'Adding tip %s'
#> Adding tip Indarctos_punjabiensis
#> [1] "Ursus_americanus" "Ursus_thibetanus" "Ursus_arctos"     "Ursus_maritimus" 
#> [5] "Ursus_spelaeus"  
#> Warning: 2 arguments not used by format 'Adding tip %s'
#> Adding tip Ursus_abstrusus
```
