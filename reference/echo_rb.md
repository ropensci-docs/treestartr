# Print RevBayes-formatted clade constriants.

Once a tip has been added to the tree, print the subtree to which the
tip was added. The output of this function is printed for use as a
RevBayes clade constraint object.

## Usage

``` r
echo_rb(tree, mrca_list, tip)
```

## Arguments

- tree:

  Tree to which the tip will be added; object of type phylo

- mrca_list:

  Vector of taxa. The added tip will subtend the MRCA of these taxa

- tip:

  Taxon which will be added to the tree.

## Value

vector A comma-separated list of all the taxa in the subtree to which
the tip was added.

## Examples

``` r
 mrca_list <- c("Ursus_arctos", "Ursus_spelaeus", "Ursus_americanus")
clade_constraint <- echo_rb(tree, mrca_list, "Ursus_abstrusus")
```
