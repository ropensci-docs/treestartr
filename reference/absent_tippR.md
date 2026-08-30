# Add tips to tree via user input

Add tips not on existing tree to the tree via user input, if they do not
have congeners on the tree. This function will generate a tree, with
nodes numbered. For each tip to be added, the user will be asked \#' to
enter the number of the node they would like the tip to subtend.

## Usage

``` r
absent_tippr(tree, absent_list)
```

## Arguments

- tree:

  Starting tree; object of type phylo

- absent_list:

  Vector of taxa in the total dataset that are not on the tree

## Value

tree Phylo object containing the starting tree, and all tips that were
added.

## Examples

``` r
if (FALSE)  new <- absent_tippr(tree, absent_list)  # \dontrun{}
```
