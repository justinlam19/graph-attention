# Exploring New Modes Of Graph Attention

### Execution

This repository contains the Jupyter Notebook, `dltheory_final_project.ipynb`, which holds all of the code for the project. It can be directly executed (running it on a GPU is recommended). Google Colab is preferred.

### Prerequisite Libraries

Required libraries are:
```
torch @ https://download.pytorch.org/whl/cu124/torch-2.6.0%2Bcu124-cp311-cp311-linux_x86_64.whl
torch-geometric==2.6.1
torch_cluster==1.6.3+pt26cu124
torch_scatter==2.1.2+pt26cu124
torch_sparse==0.6.18+pt26cu124
matplotlib==3.10.0
scikit-learn==1.6.1
ogb==1.3.6
```

This list does not include the sub-dependencies of those libraries. For a more complete reference, you can refer to `requirements.txt`, but note that this is the output of 
```
pip freeze > requirements.txt
```
which means it includes all libraries provided by Google Colab. This will likely not be needed, but it can be referenced in case of any dependency-breaking changes to the libraries.

### Pretrained Models or Datasets

No pretrained models were used.

The dataset used is `OGBG-MOLHIV`, a molecular property dataset from the Open Graph Benchmark dataset collection. It is a binary classification task to predict whether a given molecule inhibits the HIV virus. The dataset contains 41,127 graphs (each representing a molecule), with an average of 25.5 nodes per graph and 27.5 edges per graph.

The dataset is downloaded as part of the code in the Jupyter Notebook, so no additional installation is needed to get the dataset.
