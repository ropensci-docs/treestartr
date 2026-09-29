# Determine if a tip is present on a tree

Determine which tips that are not on the tree, puts them in a dataframe
if they do not have congeners on the tree

## Usage

``` r
get_lost(absent_list, tree)
```

## Arguments

- absent_list:

  Vector of taxa in the total dataset that are not on the tree

- tree:

  Starting tree; object of type phylo

## Value

not_found_df Dataframe objects expressing the tips that are not on the
tree, and don"t have congeners

## Examples

``` r
no_congeners <- treestartr:::get_lost(absent_list, tree)
```
