# SpatialAnno
SpatialAnno: Probabilistic cell/domain-type assignment of spatial transcriptomics data with SpatialAnno

SpatialAnno is a package for annotation on spatial transcriptomics datasets developed by Jin Liu's lab. It has the capability to effectively leverage a large number of non-marker genes as well as “qualitative” information about marker genes without using a reference dataset. Uniquely, SpatialAnno estimates low-dimensional embeddings for a large number of non-marker genes via a factor model while promoting spatial smoothness among neighboring spots via a Potts model

# Installation

To install the the packages "SpatialAnno", firstly, install the 'devtools' package. Besides, "SpatialAnno" depends on the 'Rcpp' and 'RcppArmadillo' package, which also requires appropriate setting of Rtools and Xcode for Windows and Mac OS/X, respectively.

install.packages("devtools")

library(devtools)

install_github("Shufeyangyi2015310117/SpatialAnno")


# Demonstration

For an example of typical SpatialAnno usage, please see our [Package vignette](https://shufeyangyi2015310117.github.io/SpatialAnno/index.html) for a demonstration and overview of the functions included in SpatialAnno.

# Usage
For usage examples and guided walkthroughs, check the `vignettes` directory of the repo. 

* [Single SRT data analysis](https://feiyoung.github.io/PRECAST/articles/PRECAST.DLPFC.html)
* [Toy examples for integrating two bathes](https://feiyoung.github.io/PRECAST/articles/PRECAST.Simu.html)
* [Integration across experimental batches](https://feiyoung.github.io/PRECAST/articles/PRECAST.BreastCancer.html)

# Analysis code

The analysis code of SpatialAnno are accessable on [code website](https://github.com/Shufeyangyi2015310117/SpatialAnno_Analysis)

## Simulation 
The simulated dataset examples were in ./Simulation/simulated_datasets folder.

Brief descriptions of simulated scripts (./Simulation/Rcode folder):


**simulated_Scenario1.R**: Anatation analysis for Scenario I. Test the robustness of SpatialAnno to the erroneous specification of the number of cell/domain types.

**simulated_Scenario2.R**: Anatation analysis for Scenario II. Evaluate the robustness of SpatialAnno to the marker gene misspecification. 

**simulated_Scenario3.R**: Anatation analysis for Scenario III. Assess the capability of SpatialAnno to utilize high-dimensional non-marker genes


## Real data analysis


Brief descriptions of real data analysis scripts (Real_data_analysis folder):

**dorsolateral_prefrontal_cortex.R**: Annotation analysis for human dorsolateral prefrontal cortex Visium data

**mouse_olfactory_bulb.R**: Annotation analysis for mouse olfactory bulb ST data

**olfactory_bulb.R**: Annotation analysis for mouse olfactory bulb Slide-seqV2 data

**mouse_embryo.R**: Annotation analysis for mouse_embryo seqFISH data



## Real data results 
The real data results were visualized with ggplot2 package (Real_data_results folder).

Brief descriptions of real data viualization  scripts:

**dorsolateral_prefrontal_cortex_viualize.R**: Visualization for human dorsolateral prefrontal cortex Visium data

**mouse_olfactory_bulb_viualize.R**: Visualization for mouse olfactory bulb ST data

**olfactory_bulb_viualize.R**:  Visualization for mouse olfactory bulb Slide-seqV2 data

**mouse_embryo.R**: Visualization for mouse_embryo seqFISH data


