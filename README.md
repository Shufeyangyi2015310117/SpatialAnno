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

# analysis code

## Simulation 
The simulated dataset examples were in ./Simulation/simulated_datasets folder.

Brief descriptions of simulated scripts (./Simulation/Rcode folder):


**simulated_Scenario1_low(middle,high).R**: Integration data analysis for Scenario 1 with three different batch effects' scales.


**simulated_Scenario2_low(middle,high).R**: Integration data analysis for Scenario 2 with three different batch effects' scales.

**simulated_Scenario3.R**: Integrative data analysis for Scenario 3.

**simulated_Scenario4.R**: Integrative data analysis for Scenario 4.

**simulated_Scenario5.R**: Integrative data analysis for Scenario 5.

## Real data analysis


Brief descriptions of real data analysis scripts (Real_data_analysis folder):

**dorsolateral_prefrontal_cortex.R**: Integration data analysis for  human dorsolateral prefrontal cortex Visium data

**mouse_liver.R**: Integration data analysis for  mouse liver ST data

**olfactory_bulb.R**:   Integration data analysis for   mouse olfactory bulb Slide-seqV2 data

**hepatocellular_carcinoma.R**: Integration data analysis for  hepatocellular carcinoma Visium data



## Real data results 
The real data results  were visualized with ggplot2 package (Real_data_results folder).

Brief descriptions of real data viualization  scripts:

**dorsolateral_prefrontal_cortex_viualize.R**: Visualization  for  human dorsolateral prefrontal cortex Visium data

**mouse_liver_viualize.R**: Visualization  for  mouse liver ST data

**olfactory_bulb_viualize.R**:  Visualization  for   mouse olfactory bulb Slide-seqV2 data

**hepatocellular_carcinoma_viualize.R**: Visualization  for  hepatocellular carcinoma Visium data


