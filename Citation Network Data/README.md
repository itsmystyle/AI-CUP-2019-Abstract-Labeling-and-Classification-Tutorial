# Extra Data - Citation Network Graph
Please download the citation network graph data from https://drive.google.com/file/d/10ygjyZ0ofNznuccC_O7CzH38QvevyJx_/view?usp=sharing

#### This citation network graph we collected from Microsoft Academic Graph
* It has ~770k nodes, 1372k edges
* ~708k nodes have Title and Abstact
* It has 1780 components and the largest component contains ~760k nodes (98.77% of nodes are linked)
* Not all paper from Train and Test set are in this graph.


#### Folder includes,
- unnormalized_title.txt:
    * This file is a sample of unnormalized paper title used to find the graph citation.

- paper_title_abstract.tsv:
    * This a tab-separated file with header.
    * It has three columns: 'PaperId', 'PaperTitle', and 'Abstract'.
    * The PaperId are defined by Microsoft Academic graph.
    * The titles in this file are "normalized". To see how the normalization done, please examine "title_converter.py" or run the command "python title_converter.py unnormalized_title.txt normalized_titles.txt".

- citation_graph.tsv:
    * This is the citation graph with nodes and edges.
    * This a tab-separated file with header.
    * It has two columns: 'PaperId', 'CitedPaperId'.
    * The PaperId are defined by Microsoft Academic Graph.
    * As an example, the row "178534    133681718" means a paper with ID 178534 cites another paper with ID 133681718.

- id_paperId.tsv:
    * This map dataset Id to Citation graph paper Id.