# Analysis of Inflammatory Biomarkers

## Project Description

Used logistic regression models, along with associated causal diagrams (DAGs),
to infer the relationship between two inflammatory biomarkers and cardiovascular
death. The biomarkers (C-reactive protein and fibrinogen) were measured as part
of a larger observational study on the elderly. The logistic models were fit
based on presupposed biological causality, to control for potential confounding
and mediating variables.

## File Details

The file `inflamm.txt` contains the data for the analysis, in tab-separated
format. 

The file inflamm_biomarker_analysis.Rmd contains the actual analysis. This
project was intended as a paper or report, and is written to summarize and
display the data, before performing a formal analysis.

The file `inflamm_biomarker_analysis.pdf` is the output of the `.Rmd` file, for
those who simply wish to view the final result, without downloading and
re-knitting the `.Rmd` file.

## Compilation Issues on Linux
As a courtesy, I thought I would let readers know that the `ggdag` package used
for creating the causal diagrams causes problems on Linux distributions. Often,
the package `V8`, called `libv8-dev` in Ubuntu respositories, must be installed
before `ggdag` and its dependencies, specifically `daggity`. Having worked on
this project cross-platform, I thought it would be best to inform interested
people of the complications of running and compiling the included code.  
