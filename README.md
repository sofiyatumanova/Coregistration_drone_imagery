# Drone Multispectral Image Co-registration in R

**Author:** Sofiya Tumanova  
**Data:** DJI multispectral TIFFs (Red, Green, NIR)  
**Requires:** R >= 4.2, `terra` package  

---

## Overview

Interactive co-registration of drone multispectral bands:

- Select the same Ground Control Point (GCP) in Red, Green, and NIR bands.
- Align Green and NIR to Red using pixel shifts.
- Crop to common overlap and save stacked raster.
- Compare before vs after co-registration in false-color and R+G / R+NIR plots.

---

## Usage

1. Download the contents of the `data/` folder.  
2. Open `clean_coregistration_script_github.R` in R or RStudio.  
3. Run the script and click on the GCP in each band.  
4. Aligned raster is saved in `output/aligned_stack.tif`.  

---

## Example Plots

| R+G Before | R+G After |
|------------|-----------|
| ![RG Before](figures/rg_before.png) | ![RG After](figures/rg_after.png) |

| R+NIR Before | R+NIR After |
|--------------|-------------|
| ![RN Before](figures/rn_before.png) | ![RN After](figures/rn_after.png) |

| False-color 3-band Before | After |
|---------------------------|-------|
| ![Before](figures/stack_before.png) | ![After](figures/stack_aligned.png) |

> Save plots in `figures/` folder using R’s `png()` if needed.

