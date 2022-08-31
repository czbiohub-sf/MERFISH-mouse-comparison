# MERFISH-mouse-comparison

Welcome to the MERFISH mouse comparison study! This repository contains Jupyter notebooks for generating figures for "Comparative analysis of MERFISH spatial transcriptomics with bulk and single-cell RNA sequencing".

# Data
The processed data to generate the figures are avilable from figshare: https://figshare.com/projects/MERFISH_mouse_comparison_study/134213. The mosaic image .tifs can be downloaded from AWS at s3://czb-tabula-muris-senis/spatial-transcriptomics/MERFISH-data/. To run the notebooks, make sure that the data folder is in the same directory that this repository is in. Make sure that all .zip files in RawData/ are unzipped into their respective folders, and that the symphony .zip is unzipped into the SingleCellData/annotated folder. See the folder structure below:

Folder structure:
```
root
├── data/
│   ├── RawData/
│   ├── BulkData/
│   ├── MosaicImages/
│   ├── SingleCellData/
│   │   ├── raw/
│   │   ├── annotated/
│   │   │   ├── symphony/
│   ├── TabulaMurisSenis/
│   ├── Visium_public/
├── MERFISH-mouse-comparison/
│   ├── notebooks/
│   │   ├── figures/
```

To run the notebooks, you will need to have the following Python packages installed:
- pandas
- matplotlib
- numpy
- scipy
- anndata
- scanpy
- squidpy
- scvi
- tifffile
- rasterio
- cv2
- shapely
- geopandas
- tqdm
- scikit-learn

In addition, the supplementary notebook for Symphony and Harmony integration requires R and the Symphony and Harmony packages to be installed.
