# Data Void Exploits: Tracking & Mitigation Strategies

## Abstract

A data void is a gap in online information, providing an opportunity for the spread of disinformation or a *data void exploit*. We introduce lightweight measures to track the progress of data void exploits and mitigation efforts in two contexts: Web search and Knowledge Graph (KG) querying. We use case studies to demonstrate the viability of these measures as data void trackers in the Web search context. To tackle data voids, we introduce an adversarial game model involving two agents: a disinformer and a mitigator. Both agents insert content into the information ecosystem to have their narrative rank higher than their counterpart in search results. At every turn, each agent chooses which content to deploy within their resource constraints, mimicking real-world situations where different entities have varying levels of influence and access to resources. Using simulations of this game, we compare and evaluate different mitigation strategies to recommend ones that maximize mitigation impact while minimizing costs.

## Repositories

This project consists of three main repositories:

1. Datavoids Explorer
2. Datavoids Web Simulator  
3. Datavoids Knowledge Graph Simulator

### Datavoids Explorer
**Repository**: [https://github.com/huda-lab/datavoids-explorer](https://github.com/huda-lab/datavoids-explorer)

This tool helps users retrieve and store the top K Google Search results over time, retrieve their content, label the content using LLMs and manual labeling, and visually display results. It was used to create the Nellie Ohr Case Study presented in our paper.
![datavoids-explorer-screenshot](/Resources/results-example-nellie.png)

### Datavoids Web Simulator 
**Repository**: [https://github.com/huda-lab/datavoids-simulator](https://github.com/huda-lab/datavoids-simulator)

This simulator models the Web search game described in the paper, where two agents compete to push the respective search rank of their narrative following the presence of a data void in the Web, represented by Wikipedia pages.

### Datavoids Knowledge Graph Simulator
**Repository**: [https://github.com/huda-lab/datavoids-kg](https://github.com/huda-lab/datavoids-kg)

This simulator models the Knowledge Graph querying game, where two agents compete to influence the link prediction ranking of their respective triples following the presence of a data void in the FB15k-237 dataset.

## Citation

If you use this code or find our work helpful, please cite our paper:

```bibtex
@inproceedings{mannino2024datavoids,
  author       = {Miro Mannino and Junior Garcia and Reem Hazim and Azza Abouzied and Paolo Papotti},
  title        = {Data Void Exploits: Tracking \& Mitigation Strategies},
  booktitle    = {Proceedings of the 33rd ACM International Conference on Information and Knowledge Management (CIKM '24)},
  year         = {2024},
  location     = {Boise, ID, USA},
  publisher    = {ACM},
  address      = {New York, NY, USA},
  pages        = {11},
  doi          = {10.1145/3627673.3679781},
  url          = {https://doi.org/10.1145/3627673.3679781},
  month        = {October 21--25}
}
```