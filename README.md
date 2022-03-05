# MERFISH-mouse-comparison

Welcome to the MERFISH mouse comparison study! This repository contains Jupyter notebooks for generating figures for "Comparative analysis of MERFISH spatial transcriptomics with bulk and single-cell RNA sequencing".

# Data
The processed data to generate the figures are avilable from figshare: https://figshare.com/projects/MERFISH_mouse_comparison_study/134213. To run the notebooks, make sure that the data folder is in the same directory that this repository is in. Make sure that all .zip files in RawData/ are unzipped into their respective folders. See the sample folder structure below:

Sample folder structure:
```
root
├── data/
│   ├── RawData/
│   ├── BulkData/
│   ├── Images/
│   ├── SingleCellData/
│   │   ├── raw/
│   │   ├── annotated/
│   ├── TabulaMurisSenis/
├── MERFISH-mouse-comparison/
│   ├── notebooks/
│   │   ├── figures/
```

Note that Figures 1, 2, and 4 are not included in this repository, as the Figure 1 was illustrated and Figures 2 and 4 utilize closed source code from Vizgen Inc. to plot some of the images.

To run the notebooks, you will need to have the following Python packages installed:
- pandas
- matplotlib
- numpy
- anndata
- scanpy
- tifffile
