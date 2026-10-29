# Detect file format of taxon file

Detect file format of the total taxon list (molecular, morphological,
and stratigraphic) and maximum age of fossil, see RevBayes total
-evidence fossil file for an example of this.

## Usage

``` r
dataf_parsr(dataf)
```

## Arguments

- dataf:

  A data frame with one column containing the taxon name of tips in
  phylogenetic tree. Optionally, a second column can indicate the
  maximum age of the tip. If the tip is extant, use 0.0 as the age. Can
  be CSV or TSV.

## Value

tax_frame Dataframe containing the total set of tips on the tree

## Examples

``` r
if (FALSE) tax_frame <- dataf_parsr(dataf) # \dontrun{}
```
