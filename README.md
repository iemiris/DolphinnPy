# DolphinnPy
DolphinnPy provides with a simple, yet efficient method for the problem of computing an (approximate) nearest neighbor in high dimensions. The algorithm is based on https://arxiv.org/abs/1612.07405, where we show linear space and sublinear query for a specific setting of parameters. 

First, N points are randomly mapped to keys in {0,1}^K, for K<=logN, by making use of the Hypeplane LSH family. Then, for a given query, candidate nearest neighbors are the ones within a small hamming radius with respect to their keys. Our approach resembles the multi-probe LSH approach but it differs on how the list of candidates is computed. 

Python 2.7
Numpy is required: numpy.org



