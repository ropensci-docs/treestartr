# Random addition of taxa

Add tips not on existing tree to the tree at random, if they do not have
congeners on the tree.

## Usage

``` r
rand_absent_tippr(tree, absent_list, echo_subtrees = NULL,
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

tree Phylo object containing the starting tree, and all tips that were
added.

## Examples

``` r
new_tree <- rand_absent_tippr(tree, absent_list)
#> Adding tips at random node: Ailurarctos_lufengensis
#> [1] 32
#> Adding tips at random node: Kretzoiarctos_beatrix
#> [1] 27
#> Adding tips at random node: Parictis_montanus
#> [1] 23
#> Adding tips at random node: Ursavus_brevirhinus
#> [1] 35
#> Adding tips at random node: Ursavus_primaevus
#> [1] 5
```
