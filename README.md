# Awesome-Graph-Contrastive-Learning
Collection of resources related with Graph Contrastive Learning.




## Contents

- [Papers](#papers)
  - [2019](#2019)
  - [2020](#2020)
  - [2021](#2021)
  - [2022](#2022)
- [Library](#library)



<a name="papers" />

## Papers

<a name="2019" />

### 2019

1. **Deep Graph Infomax** *Petar Veličković, William Fedus, William L. Hamilton, Pietro Liò, Yoshua Bengio, & R Devon Hjelm.* ICLR 2019. 
    + __Paper:__ [*OpenReview*](https://openreview.net/pdf?id=rklz9iAcKQ) | __Code:__ [*PyTorch*](https://github.com/PetarV-/DGI), [*tf_geometric*](https://github.com/CrawlScript/tf_geometric/blob/master/demo/demo_dgi.py)
    + __Method(*DGI*):__ Local-Global Mutual Information Maximization
    + __Experiment:__ 
        + __Task:__ *Transductive Node Classification* | __Datasets:__ *Cora, Citeseer, Pubmed.* | __Baselines:__ *Raw features, Label Propagation, DeepWalk, DeepWalk + features, GCN, Planetoid.*
        + __Task:__ *Inductive Node Classification* | __Datasets:__ *Reddit, PPI.* | __Baselines:__ *Raw features; DeepWalk; DeepWalk + features; GraphSAGE-GCN; GraphSAGE-mean; GraphSAGE-LSTM; GraphSAGE-pool; FastGCN; Avg. pooling.*



<a name="2020" />

### 2020

1. **InfoGraph: Unsupervised and Semi-supervised Graph-Level Representation Learning via Mutual Information Maximization** *Fan-Yun Sun, Jordan Hoffmann, Vikas Verma, Jian Tang.* ICLR 2020.
    + __Paper:__ [*OpenReview*](https://openreview.net/pdf/af171fb8c60fa180c4dcf349ccc51ff006211216.pdf) | __Code:__ [*PyTorch*](https://github.com/fanyun-sun/InfoGraph) 
    + __Method:__ Local-Global Mutual Information Maximization (Batch-wise Negative Sampling, Multi-scale), GIN
    + __Experiment:__ 
        + __Task:__ *Graph Classification* | __Datasets:__ *MUTAG, PTC-MR, RDT-B, RDT-M5K, IMDB-B, IMDB-M.* | __Baselines:__ *RandomWalk, Shortest Path Kernel, Graphlet Kernel, Weisfeiler-Lehman Sub-tree Kernel, Deep Graph Kernels, Multi-Scale Laplacian Kernel, node2vec, sub2vec, graph2vec.*
        + __Task:__ *Semi-supervised Molecular Property Prediction* | __Datasets:__ *QM9.* | __Baselines:__ *Mean-Teachers.*


1. **Contrastive Multi-View Representation Learning on Graphs** *Kaveh Hassani, Amir Hosein Khas Ahmadi.* ICML 2020.
    + __Paper:__ [*MLR*](http://proceedings.mlr.press/v119/hassani20a/hassani20a.pdf) | __Code:__ [*PyTorch*](https://github.com/kavehhassani/mvgrl)
    + __Method(*MVGRL*):__ Multi-View Local-Global Mutual Information Maximization
    + __Experiment:__ 
        + __Task:__ *Node Classification* | __Datasets:__ *Cora, Citeseer, Pubmed.* | __Baselines:__ *MLP, Iterative Classification Algorithm, Label Propagation, ManiReg, SemiEmb, Planetoid, Chebyshev, GCN, MoNet, JKNet, GAT, Linear, DeepWalk, GAE, VERSE, DGI.*
        + __Task:__ *Node Clustering* | __Datasets:__ *Cora, Citeseer, Pubmed.* | __Baselines:__ *VGAE, MGAE, ARGA, ARVGA, GALA.*
        + __Task:__ *Graph Classification* | __Datasets:__ *MUTAG, PTC-MR, IMDB-BIN, IMDB-MULTI, REDDIT-BIN.* | __Baselines:__ *Shortest Path Kernel, Graphlet Kernel, Weisfeiler-Lehman Sub-tree Kernel, Deep Graph Kernels, Multi-scale Laplacian Kernel, GraphSAGE, GIN-0, GIN-ε, GAT, RandomWalk, node2vec, sub2vec, graph2vec, InfoGraph.*


1. **GCC: Graph Contrastive Coding for Graph Neural Network Pre-Training** *Jiezhong Qiu, Qibin Chen, Yuxiao Dong, Jing Zhang, Hongxia Yang, M. Ding, Kuansan Wang, Jie Tang.* KDD 2020.
    + __Paper:__ [*ACM*](https://dl.acm.org/doi/10.1145/3394486.3403168), [*Arxiv*](https://arxiv.org/pdf/2006.09963.pdf) | __Code:__ [*DGL*](https://github.com/THUDM/GCC)



1. **Graph Contrastive Learning with Augmentations** *Yuning You, Tianlong Chen, Yongduo Sui, Ting Chen, Zhangyang Wang, Yang Shen.* NeurIPS 2020.
    + __Paper:__ [*NeurIPS*](https://papers.nips.cc/paper/2020/file/3fe230348e9a12c13120749e3f9fa4cd-Paper.pdf), [*Arxiv*](https://arxiv.org/pdf/2010.13902.pdf) | __Code:__ [*torch_geometric*](https://github.com/Shen-Lab/GraphCL)



1. **Unsupervised Graph Representation by Periphery and Hierarchical Information Maximization** *Sambaran Bandyopadhyay, Manasvi Aggarwal, M. Murty.* Arxiv 2020.
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2006.04696.pdf) 
    + __Method(*GraPHmax*):__ Periphery Information Maximization, Hierarchical Information Maximization
    + __Experiment:__ 
        + __Task:__ *Graph Classification* | __Datasets:__ *MUTAG, PTC, PROTEINS, NCI1 and NCI09, IMDB-BINARY, IMDB-MULTI.* | __Baselines:__ *Graphlet Kernel, RandomWalk Graph Kernel, Propagation Kernels, Weisfeiler-lehman Graph Kernels, AWE-DD, AWE-FB, DGCNN, PSCN, DCNN, ECC, DGK, DiffPool, IGN, GIN, 1-2-3GNN, 3WL-GNN, node2vec, sub2vec, graph2vec, DGI, InfoGraph.*
        + __Task:__ *Graph Clustering* | __Datasets:__ *MUTAG, PROTEINS, IMDB-M.* | __Baselines:__ *DGI, InfoGraph.*



1. **Graph Representation Learning via Graphical Mutual Information Maximization** *Zhen Peng, Wenbing Huang, Minnan Luo, Qinghua Zheng, Yu Rong, Tingyang Xu, Junzhou Huang.* WWW 2020.
    + __Paper:__ [*ACM*](https://dl.acm.org/doi/abs/10.1145/3366423.3380112), [*Arxiv*](https://arxiv.org/pdf/2002.01169.pdf) | __Code:__ [*PyTorch*](https://github.com/zpeng27/GMI)
    + __Method(*GMI*):__  Graphical Mutual Information
    + __Experiment:__ 
        + __Task:__ *Transductive Node Classification* | __Datasets:__ *Cora, Citeseer, Pubmed.* | __Baselines:__ *Raw Features, DeepWalk, EP-B, DGI, LP, Planetoid-T, GCN, GAT, GWNN.*
        + __Task:__ *Inductive Node Classification* | __Datasets:__ *Reddit, PPI.* | __Baselines:__ *Raw Features, DeepWalk, DeepWalk+Features, GraphSAGE-GCN, GraphSAGE-Mean, GraphSAGE-LSTM, GraphSAGE-Pool, DGI, GAT, FastGCN, GaAN.*
        + __Task:__ *Link Prediction* | __Datasets:__ *Cora, BlogCatalog, Flickr, PPI.* | __Baselines:__ *DGI.*




<a name="2021" />

### 2021


1. **Bipartite Graph Embedding via Mutual Information Maximization** *Jiangxia Cao, Xixun Lin, Shu Guo, Luchen Liu, Tingwen Liu, Bin Wang.* WSDM 2021.
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2012.05442.pdf)
    + __Method(*BiGI*):__ Local-Global Mutual Information Maximization, H-hop Enclosing Subgraph
    + __Experiment:__ 
        + __Task:__ *Top-K Recommendation* | __Datasets:__ *DBLP, ML-100K and ML-10M.* | __Baselines:__ *DeepWalk, LINE, Node2vec, VGAE, Metapath2vec, DMGI, PinSage, BiNE, GC-MC, IGMC, NeuMF, NGCF.*
        + __Task:__ *Link Prediction* | __Datasets:__ *Wikipedia.* | __Baselines:__ *DeepWalk, LINE, Node2vec, VGAE, Metapath2vec, DMGI, PinSage, BiNE, GC-MC, IGMC, NeuMF, NGCF.*



1. **How to Find Your Friendly Neighborhood: Graph Attention Design with Self-Supervision** *Dongkwan Kim, Alice Oh.* ICLR 2021
    + __Paper:__ [*OpenReview*](https://openreview.net/pdf?id=Wi5KUNlqWty) | __Code:__ [*torch_geometric*](https://github.com/dongkwan-kim/SuperGAT)
    + __Method(*SuperGAT*):__ 
    + __Experiment:__ 
        + __Task:__ *Node Classification* | __Datasets:__ *ogbn-arxiv, CS, Physics, Cora-ML,  Cora-Full, DBLP, Chameleon, Four-Univ, Wiki-CS, Photo, Computers, Flickr, Crocodile,  Cora, CiteSeer, PubMed, PPI.* | __Baselines:__ *GCN, GraphSAGE, GAT, CGAT, GLCN, LDS, GCN + GAM, GCN + NS.*
        + __Task:__ *Link Prediction* | __Datasets:__ *Cora, CiteSeer, PubMed, PPI.* | __Baselines:__ 

### 2022
<a name="2022" />

1. **CCGL: Contrastive Cascade Graph Learning** *Xovee Xu, Fan Zhou, Kunpeng Zhang, Siyuan Liu.* IEEE TRANSACTIONS ON KNOWLEDGE AND DATA ENGINEERING 2022
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2107.12576v2.pdf) | __Code:__ [*tensorflow*](https://github.com/Xovee/ccgl)
    + __Method:__(*CCGL*): Cascade Graph Learning, Contrastive learning
    
2. **SimGRACE: A Simple Framework for Graph Contrastive Learning without Data Augmentation** *Jun Xia, Lirong Wu, Jintao Chen, Bozhen Hu, Stan Z. Li.* WWW 2022 
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2202.03104v2.pdf) | __Code:__ [*pytorch*](https://github.com/junxia97/simgrace)

3. **Improving Graph Collaborative Filtering with Neighborhood-enriched Contrastive Learning** *Zihan Lin, Changxin Tian, Yupeng Hou, Wayne Xin Zhao.* WWW 2022
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2202.06200v2.pdf) | __Code:__ [*pytorch*](https://github.com/rucaibox/ncl)

4. **Knowledge Graph Contrastive Learning for Recommendation** *Yuhao Yang, Chao Huang, Lianghao Xia, Chenliang Li.* ACM SIGIR 2022
    + __Paper:__ [*Arxiv*](https://arxiv.org/pdf/2205.00976v2.pdf) | __Code:__ [*pytorch*](https://github.com/yuh-yang/kgcl-sigir22)
    
<a name="library" />

## Library
+ __PyGCL__:[*pytorch*](https://github.com/PyGCL/PyGCL)



