# conda yml files

This is a collection of various yml files that can be used to install conda env's on Hoffman2, or possibly other HPC resources

___

## H2O.ai

[H2O.ai](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/index.html)

H2O is an open source, in-memory, distributed, fast, and scalable machine learning and predictive analytics platform that allows you to build machine learning models on big data and provides easy productionalization of those models in an enterprise environment.

Both python and R APIs installed

```
conda env create -f h2oai.yml
conda activate h2oai
R -e 'install.packages("RCurl",dependencies = TRUE,repos="http://cran.r-project.org")'
R -e 'install.packages("jsonlite",dependencies = TRUE,repos="http://cran.r-project.org")'
R -e 'install.packages("h2o", type="source", repos=(c("http://h2o-release.s3.amazonaws.com/h2o/latest_stable_R")))'
```

___

## hybpiper 

[HybPiper](https://github.com/mossmatters/HybPiper)

Recovering genes from targeted sequence capture data

```
conda env create -f hybpiper-2.0.1rc.yml
conda activate hybpiper
```

___

## mdanalysis

[MDAnalysis](https://www.mdanalysis.org/)

Python package for the handling and analysis of molecular simulation data.

```
conda env create -f mdanalysis2.2.0.yml
conda activate mdanalysis
```

___

## DeepLabCut

[DeepLabCut](http://www.mackenziemathislab.org/deeplabcut)

Software package for animal pose estimation

```
conda env create -f DLC-2.2.1.1.yml
conda activate DLC
```

___

