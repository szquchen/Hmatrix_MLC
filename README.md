# Hmatrix_MLC

The code trains 3 different ML classifiers to predict whether the magnitude of an H-matrix element is greater or smaller than a threshold.

The H-matrix for the H2O vibration is used as an example. The threshold is set to 0.00001 hartree (2 cm-1). Matrix elements whose magnitude is greater than this threshold is labeled as 1, and otherwise labeled as 0. For training, 40% of the matrix elements are selected.

The ML classifiers are tested on the remaining 60% matrix elements, and the H-matrix is re-construncted using the prediction of the ML classifiers. Then the approximate eigenvalues are compared to the exact ones.
