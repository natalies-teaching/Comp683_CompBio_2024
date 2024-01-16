# Comp683: Computational Biology. (Spring 2024 iteration)
**Update Jan 10:** Our first class meeting is Thursday Jan 11 from 9:30-10:45 in Fred Brooks Building Room 007. 

This is the course page for the 2024 iteration of comp683: computational biology. The major focus of this course is on single-cell analysis and introduces the mathematical and computational infrastructure to understand common methods in the field. This course is appropriate for a broad interdiscplinary audience if you are comfortable with coding. Note that in previous years this course was numbered as Comp790-166. 
## Details

Instructor: Natalie Stanley

Email: natalies@cs.unc.edu

Time and Place: Tuesday/Thursday 9:30am-10:45am in Fred Brooks 007 (FB007). 

Info and Attributes: This is a 3-credit full-semester course and fulfills the 'Applications' category for CS students. It is a lecture-style class (I will teach the lectures) and includes two homework assignments and a course project. 

Office Hours: **Tuesday** 1pm-2pm in Sitterson 305. 

## Description
Modern, high-throughput assays allow us to efficiently profile a variety of biological processes to gain a systems-level understanding of health and disease. Recent technologies and experimental assays generate an abundance of detailed information that needs to be extracted, summarized, and interpreted. In this course we will discuss the methodology used to extract signal from (e.g. process, engineer features from, combine, etc.) data generated by some of the most cutting-edge technologies, such as single-cell assays and imaging. We will go into detail about the methods and theory underlying bioinformatics algorithms, originating from numerical linear algebra, graph-signal processing, and machine learning. While computational biology is a very broad field, we will focus here on applications in single-cell biology (CyTOF, single-cell RNA sequencing), multiomics/multi-modal analysis, systems immunology, and benchmarking. For each class of algorithms introduced for some task on biological data, we will also go over necessary theory and mathematical intuition. The course covers the foundations for biomedical data science and does not assume any biological knowledge.

## Syllabus and Course Structure
Please see the following link for a syllabus and information about key dates, homework, and the course project. [[Syllabus 2024](https://github.com/natalies-teaching/Comp683_CompBio_2024/blob/main/Syllabus_Comp683_Spring2024.pdf)]. Note that this is a lecture course with two homework assignments and a course project. 

# Topics and Tentative Schedule. 

This is the preliminary set of topics. 


| Date | Topic | Reading | Notes | Code |
|------|-------|---------|-------|------|
|Thursday, Jan 11 | Intro, Bioinformatics vs Computational Biology| [[Systems Immunology, Just Getting Started](https://www.nature.com/articles/ni.3768)], [[Grand Challenges in Single-Cell Data Science](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-1926-6)] | [[Lecture 1](https://github.com/natalies-teaching/Comp683_CompBio_2024/blob/main/Lectures/Lecture1_intro.pdf)]  | 
|Tuesday, Jan 16| Linear Algebra Review, Matrix Rank | [[SLMP. pages 10-22](https://arxiv.org/abs/2004.07984)], [[Data Matrices + Low Rank](https://arxiv.org/abs/1705.07474)] | [[Lecture 2](https://github.com/natalies-teaching/Comp683_CompBio_2024/blob/main/Lectures/Lecture2.pdf)] | [[graph tools for python](https://github.com/KrishnaswamyLab/graphtools)] |
|Thursday, Jan 18| Finish up SVD and truncated SVD; Graph Diffusion and Graph Laplacian ; Building graphs from data; Graph partitioning intro | [[LargeVis](https://arxiv.org/abs/1602.00370)], [[Random Projection Trees](https://cseweb.ucsd.edu/~dasgupta/papers/rptree-stoc.pdf)], [[Fast Unfolding of Communities in Large Networks](https://arxiv.org/abs/0803.0476)], [[Module Detection Benchmarking in Biological Data](https://www.nature.com/articles/s41592-019-0509-5)] |  | [[SNAP](https://snap.stanford.edu/)], [[Louvain](https://github.com/vtraag/louvain-igraph)], [[Leiden](https://github.com/vtraag/leidenalg)] 
|Week 2-2| Probabilistic graph partitioning (SBM, Affiliation Model))  | [[BigClam](https://dl.acm.org/doi/abs/10.1145/2433396.2433471)], [[SBM for Single-Cell](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-021-04489-7)], [[Representation Learning on Graphs](https://arxiv.org/abs/1709.05584)], [[Review: Graph Embedding in Comp Bio](https://www.frontiersin.org/articles/10.3389/fgene.2019.00381/full)]]  |  |  [[graph-tool (SBM)](https://graph-tool.skewed.de/)]  | 
|Week 3-1| Graph Embeddings with Node2vec, Intro to Single-Cell {Data Structure, Technologies, Pre-Processing}, Automating Gating and Cell-Population Discovery in Single Cell Data|[[Node2Vec](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=vQTboPUL6qIAAAAA:XQsAUtXd4MyWfj1ClUBw8FKhuPbpqO-aE2d7EDs5iX9-jJZP9BuxDbKUjg3CM69YKHALjCAKJtJx)] |   |[[node2vec](https://github.com/aditya-grover/node2vec)]   |
|Week 3-2| Gating, Graph-Based Automated Gating| [[Spade](https://www.nature.com/articles/nbt.1991)], [[Citrus](https://www.pnas.org/doi/abs/10.1073/pnas.1408792111)] [[Single-Cells, Many Features](https://www.sciencedirect.com/science/article/pii/S009286741630410X)], [[phenograph](https://www.sciencedirect.com/science/article/pii/S0092867415006376)] |  | [[phenograph](https://github.com/JinmiaoChenLab/Rphenograph)],  [[FastPG](https://github.com/sararselitsky/FastPG)], [[FCS file tutorial](https://github.com/stanleyn/fcs_tutorial)], [[Spade](https://github.com/nolanlab/spade)] |
|Week 4-1| Imputation for single-cell data, Branch Preserving Visualization for Single-Cell Data| [[MAGIC](https://www.biorxiv.org/content/10.1101/111591v1)],[[PHATE](https://www.nature.com/articles/s41587-019-0336-3)],  |  |   [[MAGIC](https://github.com/KrishnaswamyLab/MAGIC)],[[Phate](https://github.com/KrishnaswamyLab/PHATE)]  | 
|Week 4-2| Finish graph signal processing background. Start differential abundance analysis with MELD| [[MELD](https://www.biorxiv.org/content/10.1101/532846v4)] |  | [[MELD](https://github.com/KrishnaswamyLab/MELD)] [[pyGSP](https://pygsp.readthedocs.io/en/stable/)] |
|Week 5-1| No classs - wellness day. | | | |
| Week 5-2 | MELD and Cydar for condition-specific prototypical cells |  |   |  | |
|Week 6-1| Differential Abundance Analysis with Cydar | [[Cydar](https://www.nature.com/articles/nmeth.4295)] |  | [[cydar](https://www.bioconductor.org/packages/release/bioc/html/cydar.html)] |
|Week 6-2| Cydar,  Milo, Contrastive PCA for dealing with background data| [[Milo](https://www.nature.com/articles/s41587-021-01033-z)], [[Contrastive PCA](https://www.nature.com/articles/s41467-018-04608-8)] |  |  [[Milo](https://github.com/emdann/milopy)], [[Contrastive PCA](https://github.com/abidlabs/contrastive)]  | 
|Week 7-1| Finish contrastive PCA, combing disjoint single-cell datasets, sketching single-cell data  | [[Conos](https://www.nature.com/articles/s41592-019-0466-z)], [[GeoSketch](https://www.sciencedirect.com/science/article/pii/S2405471219301528)], [[Hopper](https://academic.oup.com/bioinformatics/article/36/Supplement_1/i236/5870483)] |  | [[Conos](https://github.com/kharchenkolab/conos)], [[Hopper](https://github.com/bendemeo/hopper)], [[GeoSketch](https://github.com/brianhie/geosketch)] |
|Week 7-2 | Finish sketching, start Trajectory inference and pseudo-time | [[Diffusion Maps for Differentiation](https://academic.oup.com/bioinformatics/article/31/18/2989/241305)], [[Original Diffusion Maps (Coifman)](https://papers.nips.cc/paper/2005/file/2a0f97f81755e2878b264adf39cba68e-Paper.pdf)] |   | [[Diffusion Maps -Scanpy](https://scanpy.readthedocs.io/en/latest/api/scanpy.tl.diffmap.html)], [[SLICER](https://github.com/jw156605/SLICER)] | 
 |Week 8-1| Finish Trajectory Inference - SLICER, Single-cell imaging modalities and spatial phenptyping | [[LEAPH](https://www.cell.com/cell-reports-methods/pdfExtended/S2667-2375(21)00124-7)], [[SLICER-developed at UNC](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0975-3)] |  | X |
|Week 8-2| Spatial Phenotyping with LEAPH, Pixel-level clustering (PIXIE) in IMC images, Trajectory Inference Lab Activity  | [[Pixie](https://www.biorxiv.org/content/10.1101/2022.08.16.504171v1.abstract)] | [[Notebook for trajectory activity](https://colab.research.google.com/drive/14LRc76ltDEnHi4v2jUWCS9Tad-RbXOLz?usp=sharing#scrollTo=zU82kaKhfKEN)] (Thanks to Jolene Ranek)  | [[Pixie](https://github.com/angelolab/ark-analysis)]  | 
|Week 9-1| Graph Neural Networks (GNN), Correct and Smooth Approach, GNN analysis of IMC shows spatial context doesn't always help | [[Correct and Smooth](https://arxiv.org/abs/2010.13993)], [[GNN for Spatial Context](https://www.biorxiv.org/content/10.1101/2022.12.08.519537v1)] |  | [Correct and Smooth](https://github.com/CUAI/CorrectAndSmooth)] |
|Week 9-2| No class - enjoy your spring break|  |  |  | 
|Week 10-1| No class - enjoy your spring break|  |  |  | 
|Week 10-2|Project Proposals Day 1|  |  |  | 
|Week 11-1| Project Proposals Day 2|  |  |  | 
|Week 12-1| Begin combining biological data from multiple modalities using Grassmann Embeddding| [[Subspace Merging on Grassmann Manifold](https://academic.oup.com/bioinformatics/article/35/10/1653/5134062?login=true)], [[Rayleigh Ritz Business (Spectral Clustering...](https://arxiv.org/abs/0711.0189)] |  | [[Grassmann Cluster](https://github.com/michaelsharpnack/GrassmannCluster)] | 
|Week 12-2| Graph-based multi-omics integration strategies and graph alignment | [[Mashup](https://www.cell.com/cell-systems/fulltext/S2405-4712(16)30360-X?)], [[REGAL (graph alignment)](https://gemslab.github.io/papers/heimann-2018-regal.pdf)], [[Refining Network Alignment](https://gemslab.github.io/papers/heimann-2021-RefiNA.pdf)] |  | [[Mashup](http://cb.csail.mit.edu/cb/mashup/)], [[REGAL](https://github.com/GemsLab/REGAL)] | 
|Week 13-1| Finish graph alignments with REGAL, and graph alignment refinements | [[REGAL (graph alignment)](https://gemslab.github.io/papers/heimann-2018-regal.pdf)], [[Refining Network Alignment](https://gemslab.github.io/papers/heimann-2021-RefiNA.pdf)] |  |  | 
|Week 13-2| Multiomics factor analysis (MOFA) | [[MOFA](https://www.embopress.org/doi/full/10.15252/msb.20178124)], [[MOFA+](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02015-1)] |  | [[MOFA](https://github.com/bioFAM/MOFA)] |
|Week 14-1| MOFA, MOFA+ | [[MOFA+](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02015-1)]  |   |
|Week 14-2 | Finish mutiomics factor analysis, Convex Optimization and Data Integration with ADMM ADMM | [[ADMM for ADNI](http://psb.stanford.edu/psb-online/proceedings/psb20/Brand.pdf)]  |  | | 
|Week 15-1| Finish up multimodal with temporal axis, Convex optimization    | [[Watch, Stephen Boyd ADMM](https://www.youtube.com/watch?v=Xg0ozgCXXB8)] |  |
|Week 15-2 | First Round of Project Presentations, Finish up ADMM lecture with extra time.  |  |   | 
|Week 16-1| Technical Writing in Comp Bio and Wrap-Up, Summary of the Semester wrt to graphs in biomedicine | [[Watch : How to be a Machine Learning Biologist](https://www.youtube.com/watch?v=xueh6WnpRDQ&t=1651s)], [[Graph Representation Learning in Biomedicine](https://arxiv.org/abs/2104.04883)] |  |
|Week 16-2| Second Day of Project Presentations
|May 1| Final Project Writeups Due

# Reading Questions

**Please choose 2 papers over the course of the semester to do this for, and turn them in before our class meeting 11am to natalies+comp790@cs.unc.edu**. 

1) Please explain in 2 sentences or less what the problem being solved is.

2) What were the main contributions of the authors in this work? (You can answer in a few bullet points). 

3) Please describe 1-2 computational experiments that the authors implemented to test their method.

4) Were the authors the first to attempt this particular problem? If not, did they compare their results to other baselines? Do you think that their evaluation was objective?

5) Do you think that the authors provided enough evidence for why their developed method is an important contribution? If yes, please describe their reasoning here. If you do not think they adequately justified why they worked on this particular problem, please describe your thoughts on that here. 

6) What is one follow-up idea or extension from this work? 


