# Synthetic-RNA-Seq-Raw-Counts-Generator
Generates synthetic Bulk RNA-Seq raw count data in a easy to use Google Colab Sheet, accelerated using **vectorization** & **CUDA Acceleration**

Synthetic Bulk RNA-Seq Dataset Generation
Script to generate synthetic bulk RNA-seq count data with batch effects for batch correction evaluation. An optimized version that vectorizes the count generation to improve performance.

This workflow is near instantaneous at generating data.

## Parameters:
- n_genes (int): Number of genes to simulate.
- n_samples (int): Total number of samples (should be divisible by n_batches).
- n_batches (int): Number of batches.
- de_fraction (float): Fraction of genes that are differentially expressed in treatment samples.
- fold_change (float): Fold change applied to the mean of differentially expressed genes in treatment.
- dispersion (float): Dispersion parameter for the negative binomial distribution.
- batch_effect_sigma (float): Standard deviation for batch effects (log-normal sigma).
- seed (int): Random seed for reproducibility.
## Output:
pd.DataFrame: Count matrix with gene IDs as rows and sample IDs as columns.
pd.DataFrame: Sample metadata with condition and batch information.
### Contact
For more information https://github.com/stef1949 :3
