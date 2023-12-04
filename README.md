# php2550_project3
This project is a collaboration with Dr. Jon Steingrimsson in the Brown Biostatistics Department and focuses on evaluating the performance of a prediction model in a different population than it was originally developed and/or evaluated in. 

In recent years, there have been many methods developed to help transporting measures of model performance from the source population to the target population.  Given these novel methods, it is important to apply and use them to investigate the model strengths.  In this study, a simulation study is conducted to evaluate the performance of a Cardiovascular Risk prediction model in a target population (NHANES) that differs from the population (Framingham) originally used for model development and/or evaluation. More specifically, the Brier score estimator for transportability analysis is used to evaluate the model performance. The average of the Brier scores for each simulated sample are obtained after the simulation and performance measures (Bias, Empiricial Standard Error, and Mean Squared Error) of the estimator are also calculated to further interpret the simulation result. The simulation result gives some ideas of how transportability can be affected by the varying factors such as sample sizes and covariate distributions, in the target population.

* `project3.R` performs some data pre-processing on Framingham data and NHANES data
* `project.Rmd` includes all steps for the simulation study
* Figure folder includes all plots and tables generated from this study

The R libraries required for this study are:
* library(riskCommunicator), for obtaining the Framingham data/source data
* library(nhanes), for obtaining the NHANES data/target data
* library(tidyverse), data management tool
* library(tableone), for constructing tables for data
* library(dplyr), data management tool
* library(ggplot2), result visualization tool
* library(patchwork), result visualization tool
* library(gridExtra), result visualization tool
* library(gtsummary), easily create table for data summary statistics
