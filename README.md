[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17961597.svg)](https://doi.org/10.5281/zenodo.17961597)

## Project Information Overview

### Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/UCB-stat-159-f25/final-group15/main)

---

## Overview

This repository contains an analysis of Bay Wheels bike share ridership in San Francisco from 2018 to 2024, with a focus on how weather conditions influence usage patterns. The project explores relationships between daily ridership counts and weather variables such as temperature, precipitation, and wind. The goal is to understand how environmental factors affect demand for shared micromobility and to provide clear, reproducible analysis using modern data science workflows.

---

## Data Set

The primary dataset combines Bay Wheels trip level data with daily weather observations for San Francisco.

Bay Wheels ridership data includes information on trip counts aggregated to the daily level. Weather data includes daily measures of temperature, precipitation, and other meteorological variables obtained from publicly available sources. All data are cleaned, aggregated, and merged within the project notebooks to ensure reproducibility.

---

## Project Website

The project MyST website is available at:

[https://ucb-stat-159-f25.github.io/final-group15/](https://ucb-stat-159-f25.github.io/final-group15/)

---

## Repository Structure

The repository is organized as follows.

1. data
   Contains raw and processed data files used in the analysis.

2. figures
   Contains generated figures and visual outputs.

3. notebooks
   Contains analysis notebooks.
   cleaner.ipynb performs data cleaning and daily aggregation.
   visualization_analysis.ipynb explores relationships between ridership and weather.

4. main.ipynb
   Provides the main narrative analysis and results for the project.

5. project-description.md
   Describes the final project goals and structure.

6. environment.yml
   Defines the conda environment required to run the project.

7. Makefile
   Contains commands for running notebooks and building outputs.

8. myst.yml
   Configuration file for building the MyST website.

---

## Setup and Installation

Clone the repository.

```
git clone https://github.com/UCB-stat-159-f25/final-group15.git
cd final-group15
```

Create the conda environment.

```
conda env create -f environment.yml
conda activate notebook
```

Alternatively, create the environment using Make.

```
make env
```

---

## Usage

To execute all notebooks in order, run:

```
make all
```

To build the MyST website locally, run:

```
myst build --html
```

To preview the website locally, follow the local server link printed in the terminal.

To generate a PDF from a notebook, run:

```
myst build notebook_name.ipynb --pdf
```

---

## Reproducibility

This project follows reproducible research practices.

All analysis is contained in version controlled notebooks.
The software environment is fully specified in environment.yml.
The Binder link allows the project to be launched and executed in the cloud without local setup.

---

## Testing

This project does not include unit tests. Reproducibility is ensured through deterministic data processing steps and complete environment specification.

---

## License

This project is licensed under the BSD 3 Clause License.
