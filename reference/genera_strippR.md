# Check if tip is on tree

Test which taxa in the total set of taxa are present on the tree, and
which need to be added. The tax_frame object is assumed to be a
dataframe, minimally with a column labeled "taxon". If this column does
not exist, the first column in the dataframe will be assumed to contain
the taxon information.

## Usage

``` r
genera_strippr(tree, tax_frame)
```

## Arguments

- tree:

  Starting phylogeny, of type phylo

- tax_frame:

  Total set of taxa on tree, as dataframe.

## Value

absent_list of taxa that are present in the total set of trees, but not
the starting tree

## Examples

``` r
absent_taxa <- genera_strippr(tree, tax_frame = tax_frame)
```
