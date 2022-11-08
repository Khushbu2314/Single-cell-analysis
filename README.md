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

The goal of performing dimensionality reduction is to find the approximate underlying dimensionality of the dataset.
The DimHeatmap() tries to distinguish between cells based on the PC score of the different genes.This difference is reflected in the coloring of the different groups.Here cutoff occured at pc_15(borders start to become blurry).Both cells and features are ordered according to their PCA scores. Setting cells to a number plots the ‘extreme’ cells on both ends of the spectrum, which dramatically speeds plotting for large datasets.

Elbow plots the % that each PC contributes to explaining the variation in the dataset. This means the higher the percentage, the more important the PC is.The elbow is formed from pc6 to pc10.

After elbow plot dimplot is plotted and as shwon in the image it is clear that total 6 clusters are formed.DimPlot uses UMAP by default, with Seurat clusters as identity

In feature plot two clusters were created LTB and GNLY,in single cell RNA data analysis
