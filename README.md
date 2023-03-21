# IE506 Project
## Motivation
The following is an implementation of the paper[[1]](https://www.ijcai.org/Proceedings/11/Papers/219.pdf) implementing joint feature selection and subspace learning building upon past work done on dimensionality reduction and feature selection. The core motivation for dimensionality reduction algorithms is that higher dimensional data in the input space is not good for classification due to the *curse of dimensionality*. Dimensionality reduction techniques can be broadly classified into (a) Feature selection and (b) Subspace learning.
Feature reduction is the selection of a subset of features that best represent the input data[[2]](https://www.jmlr.org/papers/volume3/guyon03a/guyon03a.pdf). On the other hand subspace learning transforms the original features to a lower dimensional subspace. Subspace learning methods include: Principal component analysis(PCA), Linear Discriminator analysis(LDA)[[3]](https://cseweb.ucsd.edu/classes/wi14/cse152-a/fisherface-pami97.pdf), Locality Preserving Projections (LPP) etc. The motivation for [[1]](https://www.ijcai.org/Proceedings/11/Papers/219.pdf) is that these methods result in new features in a lower dimensional subspace which is difficult to interpret since the original identity of the features is lost. Hence the attempt is to encourage row sparsity while learning the projection matrix in order to select relevant features and transform them simultaneously.
## Datasets
The data used is a subset of the Yale Face B dataset, and has been uploaded in the data directory of the repo.
## Results
The results obtained can be seen the the .ipynb notebook. In order to run the notebook in your system please download the data from the repo and then add the path of the data to the file_dir Variable defined in the the 1st cell of the notebook.
## Other References
1) https://www-users.cse.umn.edu/~saad/PDF/umsi-2009-31.pdf