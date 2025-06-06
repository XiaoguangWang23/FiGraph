# FiGraph
**FiGraph: A Dynamic Heterogeneous Graph Dataset for Financial Anomaly Detection**
https://dl.acm.org/doi/abs/10.1145/3701716.3715301

Graph anomaly detection (GAD) detects anomalous nodes in real-world networks by capturing topological and attributive information. Although a few of benchmark datasets are publicly available, there is a lack of dynamic heterogeneous graph datasets for advanced GAD research. To address this issue, this paper presents FiGraph, a real-world dynamic heterogeneous graph with ground-truth labels for financial anomaly detection. It consists of nine graph snapshots from 2014 to 2022 and comprises 730,408 nodes and 1,040,997 edges. There are five types of nodes and four types of edges. Only partial nodes (target nodes) need to be identified, and these nodes have multimodal attributes that incorporate tabular data and textual input. The target nodes that correspond to the same entity in different snapshots may have different labels. The remaining nodes do not need to be categorized, serving as background nodes without attributes. In addition, multiple relations can exist simultaneously between the same pair of nodes. For example, two companies may share investment and supply chain relations, while a company and a human may share both investment and related-party transaction relations. These characteristics make FiGraph more realistic and complex than existing GAD datasets, encouraging the development of more effective GAD models. This paper details the construction and properties of FiGraph and discusses promising use cases. The dataset is publicly available at: https://github.com/XiaoguangWang23/FiGraph.


## Dataset File Description
Our data is stored annually, which is beneficial for us to continue expanding this dataset year by year. Each year is considered a snapshot, and each graph snapshot is an undirected graph. The data for each snapshot is stored in a corresponding subfolder named after that year. 
* The file **"FeaturesDescription.xlsx"** provides comprehensive explanations regarding the practical significance of each feature within our dataset.

**Taking the year 2014 as an example**, the subfolder "2014" contains the snapshot data for 2014, including "edges2014.csv", "ListedCompanyFeatures772_2014.csv", and "MDA_2014.xlsx".
* **edges2014.csv**: This file consists of three columns. The first two columns represent the nodes, and the third column indicates the type of edge. Each row corresponds to an undirected edge.
* **ListedCompanyFeatures772_2014.csv**: This file stores the tabular attributes of listed company nodes, with each row representing a listed company node. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot).
* **MDA_2014.xlsx**: This file stores the textual attributes of listed company nodes. Each row represents a node of a listed company. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot). The column "ManaDiscAnal" represents the textual attribute input for each listed company node. **It should be noted that the data files for 2021 and 2022 are relatively large. Therefore, "MDA_2021.xlsx" is split into "MDA_2021_part1.xlsx" and "MDA_2021_part2.xlsx," and "MDA_2022.xlsx" is split into "MDA_2022_part1.xlsx" and "MDA_2022_part2.xlsx."**


## License
本数据集将按照“知识共享(Creative Commons)署名-非商业性使用 4.0 国际许可协议（CC BY-NC 4.0）”向您提供。您可通过访问网址 https://creativecommons.org/licenses/by-nc/4.0/legalcode.zh-Hans 了解 CC BY-NC 4.0协议内容。当您从其他地方下载或使用这些数据集时，您同意遵守 CC BY-NC 4.0 条款的约定，如果第三方对外许可的条款与 CC BY-NC 4.0相冲突，本许可条款应优先适用。我们再次重申，该数据集仅用于非商业用途，例如学术研究、教学或科学出版等。我们并未允许您将数据集或其任何衍生作品用于商业目的，例如出售数据或将其用于商业利益。[LICENSE](./LICENSE) 文件中提供了完整许可证文本的副本。使用此数据集即表示您同意这些条款。

This data set will be provided to you under the "Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)". You can learn about the CC BY-NC 4.0 agreement by visiting the URL https://creativecommons.org/licenses/by/4.0/. When you download or use these data sets from other places, you agree to abide by the terms of CC BY-NC 4.0. If the terms of a third-party external license conflict with CC BY-NC 4.0, the terms of this license shall take precedence. We reiterate that this dataset is intended for non-commercial use only, such as academic research, teaching, or scientific publishing. We do not give you permission to use the dataset or any derivative works thereof for commercial purposes, such as selling the data or exploiting it for commercial gain. A copy of the full license text is provided in the [LICENSE](./LICENSE) file. By using this dataset, you agree to these terms.


This repository contains the data that was used in our paper published at the Web Conference. If you use our data in your research, please cite our paper as follows:

**Under the following terms:**  
You must give appropriate credit. By using this dataset, you agree to these terms. This includes:
  - Citing this paper and authors as follows:    
  @inproceedings{wang2025figraph,
  title={FiGraph: A Dynamic Heterogeneous Graph Dataset for Financial Anomaly Detection},
  author={Wang, Xiaoguang and Wang, Chenxu and Liu, Huanlong and Wang, Mengqin and Qin, Tao and Wang, Pinghui},
  booktitle={Companion Proceedings of the ACM on Web Conference 2025},
  pages={813--816},
  year={2025}
}
  - Providing a link to this repository (if public).
  - You agree to abide by the terms of [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).
  - Indicating if any modifications were made (e.g., “Data were modified from the original.”) and what content has been modified.
