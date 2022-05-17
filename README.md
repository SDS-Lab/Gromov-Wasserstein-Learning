# Gromov-Wasserstein Learning
This package includes the implementation of the Gromov-Wasserstein Learning (GWL) framework for graph matching, partitioning, and node embedding.
The references are listed below. Feel free to cite them if this package is useful in your research.

Xu, Hongteng, Dixin Luo, Hongyuan Zha, and Lawrence Carin. **"Gromov-wasserstein learning for graph matching and node embedding."** In International conference on machine learning (ICML), pp. 6932-6941. PMLR, 2019. [http://proceedings.mlr.press/v97/xu19b/xu19b.pdf]

Xu, Hongteng, Dixin Luo, and Lawrence Carin. **"Scalable Gromov-Wasserstein learning for graph partitioning and matching."** Advances in neural information processing systems (NeurIPS) 32 (2019). [https://arxiv.org/pdf/1905.07645.pdf]


The examples include:
* Partition a single graph (i.e., community detection)
* Match two or more graphs (i.e., network alignment)

The package is developed on Ubuntu 18.04. 
Specifically, the baseline "metis" has been compiled as a library "libmetis.so" in the "baselines/metis-5.1.0" folder. The source code can be found at http://glaros.dtc.umn.edu/gkhome/metis/metis/download.

# Dependencies
* matplotlib
* metis (a wrapper of metis)  https://pypi.org/project/metis/
* networkx
* numpy
* pandas
* python-louvain (community) https://github.com/taynaud/python-louvain
* sklearn

Note that after install the wrapper "metis", you need to set the path of **libmetis.so** manually in **metis.py**.

# Baselines
Graph partitioning
* Metis
* Louvain
* FastGreedy
* Fluid

Graph matching
* HubAlign [https://academic.oup.com/bioinformatics/article/30/17/i438/200169]
* NETAL [https://academic.oup.com/bioinformatics/article/29/13/1654/185807]

We download these two packages from https://ttic.uchicago.edu/~hashemifar/. 
Please read the "readme" file in their folders to run these two methods.

# Citations
@inproceedings{xu2019gromov,
  title={Gromov-wasserstein learning for graph matching and node embedding},
  author={Xu, Hongteng and Luo, Dixin and Zha, Hongyuan and Duke, Lawrence Carin},
  booktitle={International conference on machine learning},
  pages={6932--6941},
  year={2019},
  organization={PMLR}
}

@inproceedings{xu2019scalable,
  title={Scalable gromov-wasserstein learning for graph partitioning and matching},
  author={Xu, Hongteng and Luo, Dixin and Carin, Lawrence},
  booktitle={Proceedings of the 33rd International Conference on Neural Information Processing Systems},
  pages={3052--3062},
  year={2019}
}

