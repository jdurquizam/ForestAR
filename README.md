# Forest Attributes Analysis in R - ForestAR

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22606690.svg)](https://doi.org/10.5281/zenodo.22606690)
[![R-CMD-check](https://img.shields.io/badge/R--Build-Passing-brightgreen.svg)]()
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> A reproducible, open-access course handbook and technical guide bridging field inventory measurements, 3D LiDAR point cloud analysis, and forest ecosystem modeling in the Peruvian Amazon.

---

## Overview

Are you ready to navigate the intersection of natural resources and computer science? This book is your guide to doing just that, equipping you with the essential skills to harness the power of data for forest management and conservation. More than just a collection of tools, this book provides a transparent and efficient approach to forestry informatics.

The curriculum guides users through raw plot cleaning, spatial point pattern modeling, canopy architecture reconstruction, and standing biomass scaling, setting the groundwork for canopy-atmosphere flux analysis.

---

## Key Modules & Topics

* **Data Standardization & Preprocessing:** Data hygiene routines, automated data validation, and reproducible tibble structures for tropical forestry plots.
* **Structural Attributes & Allometry:** Diameter at Breast Height (DBH) distributions, height-diameter modeling, basal area calculation, and stand density estimation.
* **Spatial Pattern Analysis:** Quadrat-based spatial dispersion using the **Morisita Index of Dispersion ($I_d$)** to identify clumping, random distributions, and microhabitat filtering.
* **Importance Value Index (IVI):** Synthesis of structural dominance (relative basal area), numerical composition (relative density), and landscape dispersal (relative frequency).
* **Aboveground Biomass & Carbon Scaling:** Application of pantropical allometric equations (Chave et al., 2014) and wood carbon fractions to map stand-level carbon storage and identify large-tree structural carbon hotspots.
* **3D Airborne LiDAR Visualization:** Point cloud processing with `lidR` and interactive WebGL-rendered 3D canopy models using `rgl`.

---

## Technical Stack

* **Language:** R (v4.5+)
* **Core Libraries:**
  * Spatial & LiDAR: `sf`, `lidR`, `rgl`
  * Wrangling & Visualization: `tidyverse` (`dplyr`, `ggplot2`, `tidyr`, `readr`)
  * Reporting & Tables: `bookdown`, `knitr`, `kableExtra`
* **Publishing Engine:** Pandoc, GitBook, MathJax, Giscus (GitHub Discussions API)

---

## Getting Started

### Prerequisites

Ensure you have R (>= 4.3) and RStudio installed. Install required dependencies:

```r
install.packages(c(
  "tidyverse",
  "sf",
  "lidR",
  "rgl",
  "knitr",
  "kableExtra",
  "bookdown"
))
