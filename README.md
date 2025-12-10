Bias–Variance Trade-off Illustrated via Model Capacity
Overview

This repository accompanies the tutorial “Illustrating the Bias–Variance Trade-off Through Model Capacity in Polynomial Regression.” The project demonstrates how increasing model complexity affects predictive performance, transitioning from underfitting to overfitting, and identifies the region of optimal generalisation. The aim is to provide a clear, empirical illustration of the bias–variance trade-off using controlled experiments and interpretable visualisations.

Tutorial Focus

The tutorial focuses on model capacity as the key factor influencing bias and variance. Polynomial regression models of increasing degree are trained on a synthetic regression dataset. By analysing training, validation, and test errors alongside fitted model curves, the tutorial explains how bias dominates low-capacity models, variance dominates high-capacity models, and optimal performance occurs at intermediate complexity.

Dataset

A synthetic one-dimensional regression dataset is used. Input values are sampled uniformly from a fixed interval, and targets are generated using a nonlinear function with additive Gaussian noise. The dataset is split into training, validation, and test subsets to support unbiased model evaluation and capacity selection. Using a synthetic dataset allows the true underlying function to be known, making bias and variance effects easy to interpret.

Methodology

Polynomial regression models with degrees ranging from low to high are trained using ordinary least squares. Model performance is evaluated using Mean Squared Error (MSE) on training, validation, and test sets. Error curves are plotted across model capacity, and representative model fits are visualised to qualitatively assess underfitting and overfitting behaviour.

Results

The experiments produce:

A table summarising training, validation, and test MSE across polynomial degrees

Error curves illustrating the classical U-shaped validation/test error as model capacity increases

Visual comparisons of fitted models at low, moderate, and high capacity

These results clearly demonstrate the bias–variance trade-off and confirm that intermediate model complexity yields the best generalisation performance.

Repository Structure

chandbi code.ipynb
Full, runnable Jupyter notebook containing dataset generation, model training, evaluation, and figure creation.

tutorial.pdf
The final tutorial report submitted for assessment.

figures/
Contains all figures referenced in the tutorial, including error curves and model fit visualisations.

README.md
Project overview, methodology, and usage information.

LICENSE
Specifies usage permissions for the code and materials.

Running the Notebook

The notebook is fully self-contained. Running all cells sequentially will:

Generate the synthetic dataset

Train polynomial regression models of increasing capacity

Compute training, validation, and test MSE

Produce all figures and tables used in the tutorial

All reported results are reproducible directly from the notebook.

Accessibility Considerations

To support accessible learning, all plots use high-contrast, colour-blind-safe palettes. Figure captions are descriptive and readable without reliance on colour, and tables present numerical values clearly. Headings follow a consistent hierarchy suitable for screen readers.

Licence

This project is released under the MIT License, allowing reuse, modification, and redistribution with appropriate attribution.
