# MERFISH-mouse-comparison

Welcome to the MERFISH mouse comparison study! This repository contains Jupyter notebooks for generating figures for "Concordance of MERFISH spatial transcriptomics with bulk and single-cell RNA sequencing," published in Life Science Alliance in 2022 (https://www.life-science-alliance.org/content/6/1/e202201701).

# Data

### Processed data
The processed data to generate the figures are avilable from figshare: https://figshare.com/projects/MERFISH_mouse_comparison_study/134213.

### Raw data
The raw images are available on the Tabula Muris Senis Amazon S3 bucket. Since October 2019, Tabula Muris Senis data have been made available to all users free of charge. [AWS has made the data freely available on Amazon S3](https://s3.console.aws.amazon.com/s3/buckets/czb-tabula-muris-senis/spatial-transcriptomics/) so that anyone can download the resource to perform analysis and advance medical discovery without needing to worry about the cost of storing Tabula Muris Senis data or the time required to download it. At this link you can find mosaic .tiffs of the DAPI and cell membrane antibody stains, as well as the raw .dax image files for all fluorescent channels.

### Running the notebooks
To run the notebooks, make sure that the data folder is in the same directory that this repository is in. Make sure that all .zip files in RawData/ are unzipped into their respective folders, and that the symphony .zip is unzipped into the SingleCellData/annotated folder. See the folder structure below:

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

The scRNA-seq data files from Tabula Muris Senis can be found here: https://figshare.com/articles/dataset/Tabula_Muris_Senis_Data_Objects/12654728. The bulk RNA-seq data files from Tabula Muris Senis can be found here: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE132040. The comparison with Visium datasets was performed using the mouse liver and kidney datasets from Guilliams et. al. 2022 (https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE192742) and Dixon et. al. 2022 (https://www.rebuildingakidney.org/chaise/record/#2/Common:Collection/RID=17-E9J6)
