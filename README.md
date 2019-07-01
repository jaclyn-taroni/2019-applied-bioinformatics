# MDIBL Applied Bioinformatics 2019

refine.bio and advanced machine learning topics material for MDIBL Applied Bioinformatics 2019

### R package requirements

* [`devtools`](https://cran.r-project.org/web/packages/devtools/readme/README.html)
* [`ComplexHeatmap`](https://bioconductor.org/packages/release/bioc/html/ComplexHeatmap.html)
* [`ggplot2`](https://ggplot2.tidyverse.org/#installation)
* [`dplyr`](https://dplyr.tidyverse.org/#installation)
* [`colorblindr`](https://github.com/clauswilke/colorblindr#installation) (requires `cowplot` and `colorspace`)

### Running PLIER yourself

In the interest of time, we supply a PLIER model that has been trained on [`GSE116436`](https://www.refine.bio/experiments/GSE116436/drug-induced-change-in-gene-expression-across-nci-60-cell-lines-after-exposure-to-15-anticancer-agents-for-2-6-and-24h).

If you want to run PLIER yourself (using the version we did), you install it using the [`devtools`](https://cran.r-project.org/web/packages/devtools/index.html) package with the following command:

```R
devtools::install_github('wgmao/PLIER', 
                         ref = 'a2d4a2aa343f9ed4b9b945c04326bebd31533d4d', 
                         dependencies = TRUE)
```
Examples of how to run PLIER yourself can be found in the `PLIER` package vignette and in the Childhood Cancer Data lab training workshop material: 

* [Medulloblastoma PLIER notebook](https://alexslemonade.github.io/training-modules/machine-learning/03-medulloblastoma_PLIER.nb.html)
* Upstream processing (e.g., conversion between gene identifiers) can be found [this notebook](https://alexslemonade.github.io/training-modules/machine-learning/01-medulloblastoma_data_prep.nb.html)
