# MindSpore implementation of EvoExplore

[pytorch implementation](https://github.com/zjs123/EvoExplore)

Paper: "EvoExplore: temporal knowledge graph representation learning via co-evolution modelling"

In this paper, we propose a novel framework to learn representations for temporal knowledge graph via modelling its local and global structure co-evolution, and this repository contains the  benchmark datasets used in the paper and the implementation of our proposed framework.

<p align="center"><img src="Evo.PNG"/></p>

We firstly regard the local structure evolution as the establishment process of relations between different entities, and propose a novel hierarchical-attention-based temporal point process to model the establishment of each relation. This helps our framework to capture the evolutionary nature of TKG from a local perspective. Secondly, we regard the global structure evolution as its time-evolving community partition, and design a soft modularity as the metric to model the community structure in TKG. By jointly maximizing the soft modularity in each timestamp, our framework captures the evolutionary nature of TKG from a global perspective. Finally, we employ a multi-task loss function to jointly optimize the above two parts, which allows EvoExplore to capture the co-evolutionary pattern between local and global structure evolutions. Experimental results demonstrate the superiority of our proposed method compared with existing baselines.

If you make use of this code in your work, please cite the following paper:

```
@inproceedings{Zhang2021EvoExplore,
  title={EvoExplore: temporal knowledge graph representationlearning via co-evolution modelling},
  author={Jiasheng Zhang, Yongpan Sheng, Shuang Liang and Jie Shao},
  booktitle={},
  year={2021}
}
```
