# MLNS-Final-Project

In this project, we explore several approaches to optimise target re-identification (re-ID) as a re-ranking problem. Our work consisted in trying different methods to re-rank the re-ID results. 

# Datasets

We will be testing our work on Market-1501 and VeriWild

To run reranking evaluation:
1. Place dataset files (issued from the feature extraction) under 'dataset/' folder:
The dataset structure should be like:

```bash
datasets/
    Market/
        camids.pkl
        feat.pkl
        ids.pkl
``` 
We used https://github.com/JDAI-CV/fast-reid for the feature extraction part. 

For visualization, you should also download the Market-1501 dataset (images). 
# Requirements 

* dgl
* Pytorch 
* scikit-learn

# GNN based reranking
The code has been included in `/extension`. To compile it:

```shell
cd extension
sh make.sh
```
To run reranking evaluation:
1. Place dataset files under 'dataset/' folder:
The dataset structure should be like:

```bash
datasets/
    Market/
        camids.pkl
        feat.pkl
        ids.pkl
``` 
2. python run.py
Ps: Reranking runs only on GPU

# Members 
Chady Raach 
Mehdi Zemni 
Marah Gamdou
