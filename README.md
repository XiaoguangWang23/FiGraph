# FiGraphN
**FiGraph: A Dynamic Heterogeneous Graph Dataset for Financial Anomaly Detection**

## Description
* **'edges2014.csv', 'edges2015.csv', 'edges2016.csv', 'edges2017.csv', 'edges2018.csv', 'edges2019.csv', 'edges2020.csv', 'edges2021.csv', 'edges2022.csv'** respectively store one graph snapshot. Each graph snapshot is an undirected graph. Each CSV file consists of three columns, with the first two columns being nodes and the third column being the type of edge. Each row represents an undirected edge.

* **'ListedCompanyFeatures772.csv'** stores the tabular attributes of listed company nodes, with each row representing a listed company node. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot).

* **MDA.xlsx** stores the textual attributes of listed company nodes. Each row represents a node of a listed company. In this file, column "nodeID" represents the node ID of the listed company, and column "Label" represents the ground truth labels of the listed company, The column "Year" represents the year (snapshot). The column "ManaDiscAnal" represents the textual attribute input for each listed company node.


## License
This dataset is licensed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) License](https://creativecommons.org/licenses/by/4.0/). A copy of the full license text is provided in the [LICENSE](./LICENSE) file.


**Under the following terms:**
- **Attribution** — You must give appropriate credit. This includes:
  - Citing the authors as follows:
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
  - Including a link to the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).
  - Indicating if any modifications were made (e.g., “Data were modified from the original.”).

**No Additional Restrictions:**
- You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

**For More Information:**
- The full legal code of the license is available in the [LICENSE](./LICENSE) file and at [https://creativecommons.org/licenses/by/4.0/legalcode](https://creativecommons.org/licenses/by/4.0/legalcode).

By using this dataset, you agree to these terms.
