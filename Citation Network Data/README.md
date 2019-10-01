# Extra Data
Please download the citation graph data from https://drive.google.com/file/d/10ygjyZ0ofNznuccC_O7CzH38QvevyJx_/view?usp=sharing

unnormalized_title.txt:
    * This file is a sample of unnormalized paper title used to find the graph citation.

paper_title_abstract.tsv:
    * This a tab-separated file with header.
    * It has three columns: 'PaperId', 'PaperTitle', and 'Abstract'.
    * The PaperId are defined by Microsoft Academic graph.
    * The titles in this file are "normalized". To see how the normalization done, please examine "title_converter.py" or run the command "python title_converter.py unnormalized_title.txt normalized_titles.txt".

citation_graph.tsv:
    * This is the citation graph with nodes and edges.
    * This a tab-separated file with header.
    * It has two columns: 'PaperId', 'CitedPaperId'.
    * The PaperId are defined by Microsoft Academic graph.
    * As an example, the row "178534	133681718" means a paper with ID 178534 cites another paper with ID 133681718.

id_paperId.tsv:
    * This map dataset Id to Citation graph paper Id.
