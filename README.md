# Large-scale clustering in Bioconductor

## Key resources

- Workshop material: [pkgdown website](https://stephaniehicks.com/biocdemo)
- Code: [GitHub](https://github.com/stephaniehicks/biocdemo)

## Demo description

This website gives a demo of large-scale clustering in the Bioconductor using the *DelayedArray* framework. 
*DelayedArray* is like an ordinary array in R, but allows for the data to be in-memory, on-disk in a file, or even hosted on a remote server. Specifically, we present two forms of dimensionality reduction : 

1. `scran` normalization + PCA
2. `glmpca` with `scry`

Using these reduced dimensions, we present two types of clustering: 

1. SNN + Louvain clustering
2. mini-batch _k_-means (`mbkmeans`)

### Instructors

- [Stephanie C. Hicks](https://www.stephaniehicks.com) (shicks19@jhu.edu)
- [Davide Risso](https://drisso.github.io) (risso.davide@gmail.com)

### *R* / *Bioconductor* packages used

These packages are the focus of this workshop:

- `SingleCellExperiment`
- `TENxPBMCData`
- `scater`
- `scran`
- `scry`
- `mbkmeans`

Please see the workshop [`DESCRIPTION`](https://github.com/stephaniehicks/biocdemo/blob/main/DESCRIPTION) for a full list of dependencies.


## Installation

This demo uses Bioconductor version 3.12.
This is the current 'release' version of Bioconductor, which can be installed following [these instructions](https://bioconductor.org/install/).

You can then install the packages necessary for this workshop using the following:

```
library(BiocManager)
install(c("SingleCellExperiment", "TENxPBMCData", "scater", "scran",
  "scry", "mbkmeans"))
```
