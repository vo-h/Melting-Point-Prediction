# Melting-Point-Prediction

This project aims to predict the melting point of a given organic molecule. I plan to try out both traditional machine learning approaches (PyCaret) and neural networks (Torch Drug).

## data

Folder containing Google Colab notebook I used to obtain & clean data from PubChem. Also, it contains .csv files of clean data. There are ~17000 molecules that have recorded melting points. Some of them are inorganic. Some have discrepancies in the recorded melting points. After cleaning, there are ~4000 organic molecules that can be used for training.

## mp_traditional.ipynb

Using PyCaret and generated features from RDKit, it was determined that LightGBM performs the best with RMSE ~ 47 and MAE ~ 35. I have yet to do further analysis on the resulting model. At first glance, though, this is not the best result. This [paper](https://pubs.acs.org/doi/10.1021/ci5005288), for example, got an RMSE ~ 37. But it was on a larger yet more restrictive dataset (~21000 drug-like molecules), and the feature space is much much more massive (they used different packages to generate descriptors, and one of them could generate ~5000 descriptors).

## mp_gnn.ipynb

Coming up next....
