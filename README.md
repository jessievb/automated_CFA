# Automated analysis of colony formation assay experiments

Colony forming assays are used to determine colony forming potential of stem cells such as primary skin stem cells (keratinocytes). Immuno-staining of a differentiation marker in these colonies allows evaluation of both colony-forming potential as well as differentiation status of the cells at a molecular level. We created a pipeline using CellProfiler and R, to analyze DRAQ5 (DNA) and TGM1 (differentiation marker) stained keratinocyte colonies. This pipeline allows visualization of colony number, colony area, colony radius, the intensity of differentiation marker TGM1 per condition.

# Description workflow

## CellProfiler

Use the .cppipe pipeline to process all images (700 and 800 channel BW images). Note that a mock-stained plate is needed for this CellProfiler Pipeline.

The pipeline saves information in files like "coloniesDraq5.csv" and "Grid_6wells.csv" files. These files are used in the R-script described below. 

## Data analysis in R

R-notebook contains all scripts to import the data and visualize colony number, colony area, colony radius and differentiation marker intensity
