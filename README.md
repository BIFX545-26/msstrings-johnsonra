# MSstrings


MSstrings is a package that will read in Spectronaut-formatted peptides
with or without protein modifications and display them nicely.

## Installation

MSstrings can be installed from GitHub using the following command:

``` r
devtools::install_github('BIFX545-26/msstrings-johnsonra')
```

## Example

This package comes with a sample data set, which we import and display
below.

``` r
library(MSstrings)

data("MSfrags")
parse_mods(MSfrags)
```

    22-letter AAString object
    seq: MDYQVSSPIYDINYYTSEPCQK
              |
              Glycosylation

    28-letter AAString object
    seq: LLPPLYSLVFIFGFVGNMLVILILINCK
                          |
                          Oxidation

    64-letter AAString object
    seq: SMTDIYLLNLAISDLFFLLTVPFWAHYAAAQWDFGNTMCQLLTGLYFIGFFSGIFFIILLTIDR
              |                        |
              |                        Deamidation
              Acetylation

    28-letter AAString object
    seq: TVTFGVVTSVITWVVAVFASLPGIIFTR
      No modifications
