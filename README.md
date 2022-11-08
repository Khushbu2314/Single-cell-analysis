# Single-cell-analysis
Single cell RNA-seq data used here is generated using the 10X genomics platform
Single cell RNA sequencing (scRNA-seq) is a novel technique for extracting more detailed information from genome,scRNA-seq is useful in case of heterogeniety of cells and developmental studies.

Here files taken are GSM5712850_CC04_barcodes.tsv.gz as my barcodes.tsv.gz ,GSM5712850_CC04_features.tsv.gz	as features.tsv.gz and 
GSM5712850_CC04_matrix.mtx.gz as matrix.mtx.gz files.

And some of the plots are created such as dimheat plot,feature scatter plots, elbow plot etc.

Interpretation: 
Each dot shows thevalue of the individual cell.
In graph nfeature_RNA ,nCount_RNA and percent_mt are shown,where:

The nfeature_RNA shows number of detected genes for every cell,the average number of genes per cell is about 200-600 
The nCount_RNA shows the no .of genes detected in a cell which is densely located is around approx.,500-2000 and percent_mt shows the mitochondrial percentage according to the density is approx 5-7%

The feature scatter plots shows the correlation,here plot1 value shown is -0.31(percent.mt) and plot2 has value 0.93(n_Feature_RNA) .

In variable feature plot , they have shown us the variable count and non variable count of the top 10 genes mentioned.

DimPlot is used to visualize all reduced representations,DimPlot has built-in hiearachy of dimensionality reductions it tries to plot: first, it looks for UMAP, then (if not available) tSNE, then PCA.The goal of performing dimensionality reduction is to find the approximate underlying dimensionality of the dataset.



