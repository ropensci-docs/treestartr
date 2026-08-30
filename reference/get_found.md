# Get dataframe of tips that do not have congeners on tree.

Determine which tips that are not on the tree, and checks if they have
congeners on the tree.

## Usage

``` r
get_found(absent_list, tree)
```

## Arguments

- absent_list:

  Vector of taxa in the total dataset that are not on the tree

- tree:

  Starting tree; object of type phylo

## Value

found_df Dataframe objects expressing the tips that are not on the tree,
if they have congeners on the tree

## Examples

``` r
has_congeners <- treestartr:::get_found(absent_list, tree)
```
