# Determine which tips are not on the tree, and get their genera.

Determine which tips are not on the tree, and get their genera.

## Usage

``` r
make_absentdf(absent_list)
```

## Arguments

- absent_list:

  Vector of taxa in the total dataset that are not on the tree

## Value

absent_df Dataframe objects expressing which tips are in the total set
but not the tree, and their genera

## Examples

``` r
not_present <- treestartr:::make_absentdf(absent_list)
```
