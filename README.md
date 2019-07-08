# MDIBL Applied Bioinformatics 2019

[refine.bio](https://www.refine.bio/) and advanced machine learning topics material for [MDIBL Applied Bioinformatics 2019](https://mdibl.org/course/applied-bioinformatics-2019/)

### R package requirements

* [`devtools`](https://cran.r-project.org/web/packages/devtools/readme/README.html)
* [`ComplexHeatmap`](https://bioconductor.org/packages/release/bioc/html/ComplexHeatmap.html)
* [`ggplot2`](https://ggplot2.tidyverse.org/#installation)
* [`dplyr`](https://dplyr.tidyverse.org/#installation)
* [`colorblindr`](https://github.com/clauswilke/colorblindr#installation) (requires `cowplot` and `colorspace`)

Notebooks will check if these packages are installed and if not, install them.

### Notebooks

1. [Making a heatmap of refine.bio data using `ComplexHeatmap`](https://jaclyn-taroni.github.io/2019-applied-bioinformatics/01-refinebio_heatmap.nb.html)
2. [Exploring treatment of NCI-60 cell lines with `PLIER`](https://jaclyn-taroni.github.io/2019-applied-bioinformatics/02-nci60_explore_plier.nb.html)

### Running PLIER yourself

In the interest of time, we supply a Pathway-Level Information ExtractoR (PLIER) model ([Mao et al. _bioRxiv._ 2017.](https://doi.org/10.1101/116061)) that has been trained on [`GSE116436`](https://www.refine.bio/experiments/GSE116436/drug-induced-change-in-gene-expression-across-nci-60-cell-lines-after-exposure-to-15-anticancer-agents-for-2-6-and-24h).

If you want to run PLIER yourself (using the version we did), you can install it using the [`devtools`](https://cran.r-project.org/web/packages/devtools/index.html) package with the following command:

```R
devtools::install_github('wgmao/PLIER', 
                         ref = 'a2d4a2aa343f9ed4b9b945c04326bebd31533d4d', 
                         dependencies = TRUE)
```
Examples of how to run PLIER yourself can be found in the `PLIER` package vignette and in the Childhood Cancer Data lab training workshop material: 

* [Medulloblastoma PLIER notebook](https://alexslemonade.github.io/training-modules/machine-learning/03-medulloblastoma_PLIER.nb.html)
* Upstream processing (e.g., conversion between gene identifiers) can be found [this notebook](https://alexslemonade.github.io/training-modules/machine-learning/01-medulloblastoma_data_prep.nb.html)
