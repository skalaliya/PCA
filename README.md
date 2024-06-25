# Principal Component Analysis (PCA)

YouTube Link: https://github.com/skalaliya/PCA

**Principal Component Analysis (PCA)** is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components.

## How does PCA work?

1. **Standardization**: The first step in PCA is to standardize the feature set. Standardization is all about scaling your data in such a way that all variables and their values lie within a similar range.

2. **Covariance Matrix computation**: The next step is to find the covariance matrix of the standardized feature set. The covariance matrix is a p × p symmetric matrix (where p is the number of dimensions) that has as entries the covariances associated with all possible pairs of the initial variables. For each pair of variables, the covariance matrix shows how those two variables vary together.

3. **Compute the Eigenvalues and Eigenvectors**: The next step is to find the eigenvalues and the corresponding eigenvectors of the covariance matrix. The eigenvectors of the Covariance matrix are actually the directions of the axes where there is the most variance(most information) and that we call Principal Components. And eigenvalues are simply the coefficients attached to eigenvectors, which give the amount of variance carried in each Principal Component.

4. **Sort Eigenvalues and their corresponding Eigenvectors**: Next we make a list of (eigenvalue, eigenvector) tuples and sort these tuples from high to low.

5. **Choose first k eigenvectors**: This step is also called as the extraction of the principal components. We choose the first k eigenvectors, which corresponds to the k largest eigenvalues, where k is the dimensionality of the new feature subspace (k≤p).

6. **Transform original dataset**: In the last step, we will use the k eigenvectors selected to transform our original dataset of dimension p to a new subspace of dimension k.

## Applications of PCA

PCA is predominantly used as a dimensionality reduction technique in domains like facial recognition, computer vision and image compression. It is also used for finding patterns in data of high dimension in the field of finance, data mining, bioinformatics, psychology, etc.
