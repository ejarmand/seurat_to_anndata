# seurat_to_anndata

A script to convert a seurat object saved as an RDS to an anndata for scanpy.

### NOTE
this script will ONLY preserve the default assay, as well as the metadata.

## installing necesary packages
This assumes you have conda installed
1. set up conda
```
conda create -n seurat_to_anndata
conda activate seurat_to_anndata
conda install -c bioconda r-seurat anndata scater zellkonverter
conda install -c conda-forge r-reticulate  
```
2. download script
git clone this repo

## Usage
```
conda activate seurat_to_anndata 
R seurat_to_anndata seurat_obj.rds anndata_out.h5ad
```
