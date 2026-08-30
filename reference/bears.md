# bears

A dataset containing 18 taxa and 62 characters for bears

## Usage

``` r
data(bears)
```

## Format

A collection of objects representing function inputs:

- tax_frame:

  a two-column dataframe of taxon names and ages

- absent_list:

  A list of taxa in the total data set, but are not on the tree

- mrca_df:

  a two-column dataframe of taxa to be placed, and a set of taxa that
  indicate the MRCA which they will subtend

- tree:

  A phylogenetic tree to which tips will be added

## Source

<https://github.com/revbayes/revbayes_tutorial/tree/master/RB_TotalEvidenceDating_FBD_Tutorial/data>
