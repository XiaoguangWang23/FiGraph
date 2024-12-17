# Folder data
## **overall.**
Folder 'data' stores the edges data and node attribute data of FiGraph. To fill the above space, this paper presents FiGraph, a real-world and large-scale dynamic heterogeneous graph collected from the Chinese capital market. It consists of 9 graph snapshots from 2014 to 2022 and comprises 730,408 nodes and 1,040,997 edges. Figure 1 illustrates an example of FiGraph. There are mainly five types of nodes: listed companies, unlisted companies, audit institutions, human, and others. The primary goal is to train a GAD model to predict whether a listed company involves a financial fraud. In this specific problem, listed companies are target nodes (TNs), and the rest are background nodes (BNs). Each graph comprises four types of edges: investments, related-party transactions, supply chains, and audit relations. Listed companies exert the most significant impact on the entire capital market and are the focus of regulatory authorities. They are legally required to publish annual financial reports annually in order to be scrutinized for fraudulent activities. Therefore, these nodes have rich attribute information. However, unlisted companies are not obliged to disclose their financial statements, making it challenging to obtain their financial attributes. And the attributes of the remaining nodes are also difficult to obtain in the real world. Therefore, FiGraph is a partially-attributed dynamic heterogeneous graph, where listed company nodes (TNs) possess rich attributes while the remaining nodes lack such information. This dataset can enrich the diversity of current GAD datasets and significantly promote GAD research. 

## Edges
**'edges2014.csv', 'edges2015.csv', 'edges2016.csv', 'edges2017.csv', 'edges2018.csv', 'edges2019.csv', 'edges2020.csv', 'edges2021.csv', 'edges2022.csv'** respectively store one graph snapshot. Each graph snapshot is an undirected graph. Each CSV file consists of three columns, with the first two columns being nodes and the third column being the type of edge. Each row represents an undirected edge.

## Complete Raw Node attributes
**'ListedCompanyFeatures772. csv'** stores the complete raw attributes of all target nodes accross on 9 snapshots. In 'ListedCompanyFeatures772. csv':

* 'nodeID' column is the ID code of the target node, 
* 'Year' represents the year.
* 'Label' represents the label, 1 represents normal while 0 represents fraud.

## Features file and feature selection 
* **ListedCompanyFeatures772.csv'** stores the complete raw attributes of all target nodes and detailed attribute descriptions available in **"FeaturesDescription.xlsx"**.



# Attribute Description
* Details in **'FeaturesDescription.xlsx'** for all attributes of target nodes.
