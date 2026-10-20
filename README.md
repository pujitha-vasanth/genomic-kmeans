# Finding Codons with PCA and K-Means

Can unsupervised learning rediscover that DNA is read in three-letter words (codons), with no biology given to it?

Using the genome of the bacterium *Caulobacter crescentus* (`ccrescentus.fa`):

1. Cut the sequence into 300-letter fragments
2. For word lengths 1 to 4, count how often every possible word appears in each fragment
3. Standardise the frequency tables and project each to two dimensions with PCA
4. Cluster with K-means

Only the three-letter word length produces clear, separated clusters (about 7), which supports the codon structure of the genetic code.

## Files

- `Genomic Data KMeans Clustering.ipynb`: the analysis
- `ccrescentus.fa`: the genome sequence (FASTA)

## Stack

Python, pandas, NumPy, scikit-learn, Matplotlib
