---
layout: default
title: Plant3G
subtitle: plant breeding toolset
---

## Overview

The **Plant3G** package was designed to be a transparent engine for NGS-enabled genomic selection and genome-wide association studies.



## Motivation

One of the difficulties with extending Sweave is we have to copy a large
amount of code from the **utils** package (the file `SweaveDrivers.R` has
more than 700 lines of R code), and this is what the two packages mentioned
above have done. Once the code is copied, the package authors have to pay
close attention to what is changing in the version in official R --
apparently an extra burden. The **knitr** package tried to modularize the
whole process of weaving a document into small manageable functions, so it
is hopefully easier to maintain and extend (e.g. easy to support HTML
output); on the other hand, **knitr** has many built-in features and it
should not be the case to have to hack at the core components of this
package. By the way, several FAQ's in the Sweave manual are solved in
**knitr** directly.

> Let us change our traditional attitude to the construction of programs:
> Instead of imagining that our main task is to instruct a computer what to
> do, let us concentrate rather on explaining to humans what we want the
> computer to do. <cite>-- Donald E. Knuth, Literate Programming, 1984</cite>

## Features

The ideas are borrowed from other packages, and some of them are
re-implemented in a different way (like cache). A selected list of features
include:


## Basic usage and data formats <a id="basic"></a>
   - `DSF`: density SNP format (self defined)
   - `VCF`: variant call format
   - `HapMap`: 

 
## SNP imputation <a id="impute"></a>
   - `diallel`: from parental high density SNP panel to F1 hybrids. support several downstream analysis software, such as PLINK, SNPTEST, GenSel, ... 
   - `RIL`: from parental high density SNP panel to RILs based on tagging SNPs of RILs.
   - `F1BCn`: from parental high density SNP panel to progenies of the F1BCn based on GBS panel of F1BCn individuals (not implemented yet)

    
## SNP manipulation  <a id="manipulation"></a>




