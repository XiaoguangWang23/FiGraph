# FiGraph
Our Paper: 

**FiGraph: A Dynamic Heterogeneous Graph Dataset for Financial Anomaly Detection**

This paper presents FiGraph, a real-world dynamic heterogeneous graph with ground-truth labels for financial anomaly detection. It consists of nine graph snapshots from 2014 to 2022 and comprises 730,408 nodes and 1,040,997 edges. There are five types of nodes and four types of edges. Only partial nodes (target nodes) need to be identified, and these nodes have multimodal attributes that incorporate tabular data and textual input. The target nodes that correspond to the same entity in different snapshots may have different labels. The remaining nodes do not need to be categorized, serving as background nodes without attributes. In addition, multiple relations can exist simultaneously between the same pair of nodes. For example, two companies may share investment and supply chain relations, while a company and a human may share both investment and related-party transaction relations. These characteristics make FiGraph more realistic and complex than existing graph anomaly detection (GAD) datasets, encouraging the development of more effective GAD models. This paper details the construction and properties of FiGraph and discusses promising use cases. The dataset is publicly available at: https://github.com/XiaoguangWang23/FiGraph.


## Dataset File Description
* **'edges2014.csv', 'edges2015.csv', 'edges2016.csv', 'edges2017.csv', 'edges2018.csv', 'edges2019.csv', 'edges2020.csv', 'edges2021.csv', 'edges2022.csv'** respectively store one graph snapshot. Each graph snapshot is an undirected graph. Each CSV file consists of three columns, with the first two columns being nodes and the third column being the type of edge. Each row represents an undirected edge.

* **'ListedCompanyFeatures772.csv'** stores the tabular attributes of listed company nodes, with each row representing a listed company node. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot).

* **'MDA.xlsx'** stores the textual attributes of listed company nodes. Each row represents a node of a listed company. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot). The column "ManaDiscAnal" represents the textual attribute input for each listed company node.


## License
本数据集将按照“知识共享(Creative Commons)署名-非商业性使用 4.0 国际许可协议（CC BY-NC 4.0）”向您提供。您可通过访问网址 https://creativecommons.org/licenses/by-nc/4.0/legalcode.zh-Hans 了解 CC BY-NC 4.0协议内容。当您从其他地方下载或使用这些数据集时，您同意遵守 CC BY-NC 4.0 条款的约定，如果第三方对外许可的条款与 CC BY-NC 4.0相冲突，本许可条款应优先适用。我们再次重申，该数据集仅用于非商业用途，例如学术研究、教学或科学出版等。我们并未允许您将数据集或其任何衍生作品用于商业目的，例如出售数据或将其用于商业利益。[LICENSE](./LICENSE) 文件中提供了完整许可证文本的副本。使用此数据集即表示您同意这些条款。

This data set will be provided to you under the "Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)". You can learn about the CC BY-NC 4.0 agreement by visiting the URL https://creativecommons.org/licenses/by/4.0/. When you download or use these data sets from other places, you agree to abide by the terms of CC BY-NC 4.0. If the terms of a third-party external license conflict with CC BY-NC 4.0, the terms of this license shall take precedence. We reiterate that this dataset is intended for non-commercial use only, such as academic research, teaching, or scientific publishing. We do not give you permission to use the dataset or any derivative works thereof for commercial purposes, such as selling the data or exploiting it for commercial gain. A copy of the full license text is provided in the [LICENSE](./LICENSE) file. By using this dataset, you agree to these terms.


**Under the following terms:**  
You must give appropriate credit. By using this dataset, you agree to these terms. This includes:
  - Citing this paper and authors as follows:
    - **Xiaoguang Wang** (wangxg@stu.xjtu.edu.cn, [ORCID: 0000-0002-6060-5883])  
      *Xi'an Jiaotong University, Xi'an, China*
    - **Chenxu Wang** (Corresponding author, cxwang@mail.xjtu.edu.cn, [ORCID: 0000-0002-9539-5046])  
      *Xi'an Jiaotong University, Xi'an, China*
    - **Huanlong Liu** (hlliu@stu.xjtu.edu.cn, [ORCID: 0009-0009-7932-8706])  
      *Xi'an Jiaotong University, Xi'an, China*
    - **Mengqin Wang** (wmengqin@stu.xjtu.edu.cn, [ORCID: 0009-0005-8130-0623])  
      *Xi'an Jiaotong University, Xi'an, China*
    - **Tao Qin** (qin.tao@mail.xjtu.edu.cn, [ORCID: 0000-0002-7674-698X])  
      *Xi'an Jiaotong University, Xi'an, China*
    - **Pinghui Wang** (phwang@mail.xjtu.edu.cn, [ORCID: 0000-0002-1434-837X])  
      *Xi'an Jiaotong University, Xi'an, China*

  - Providing a link to this repository (if public).
  - You agree to abide by the terms of [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).
  - Indicating if any modifications were made (e.g., “Data were modified from the original.”) and what content has been modified.
