# Bioinformatics-Projects
This repository houses all my Bioinformatics practice projects using tools and biological databases. Projects you will find in this repository:
* Pairwise Sequence Alignment
* Multiple Sequence Alignment
* Phylogenetic Tree Reconstruction
* Building Phylogenetic trees using Mega
* Unsupervised Machine Learning and Clustering Problem
* Using K-means in Weka

Below are the introductory or short explanatory sessions of the project.
## Pairwise Sequence Alignment
Pairwise Sequence Alignment is a type of sequence alignment used to identify similar regions that may indicate relationships between two biological sequences. This relationship could be functional, structural, evolutionary, or a combination of two or more of these relationships. The biological sequences could also be nucleic acid or protein. As opposed to Pairwise Sequence Alignment, Multiple Sequence Alignment is the alignment of more than 2 biological sequences of similar length. 
Alignment can either be Global or Local. Global alignment matches the entire length of the sequences, while Local alignment looks for sub-sequences of both sequences and matches them optimally to each other.  
**There are different tools that can be used for the Global alignment of paired sequences:** 
* The EMBOSS Needle which uses the Needleman-Wunsch algorithm
* The EMBOSS Stretcher which applies the modification of the Needleman-Wunsch algorithm and allows larger sequences to be aligned
* The GGSEARCH2SEQ which finds an optimal global alignment using the Needleman-Wunsch algorithm.

  **There are also different tools that can be used for the Local alignment of paired sequences:**

  
* The EMBOSS Water which uses the Smith-Waterman algorithm (modified for speed enhancements) to calculate the local alignment of two sequences.
* The EMBOSS Matcher which identifies local similarities between two sequences using a rigorous algorithm based on the LALIGN application.
* The LALIGN which finds internal duplications by calculating non-intersecting local alignments of protein or DNA sequences
* The SSEARCH2SEQ finds an optimal local alignment using the Smith-Waterman algorithm.
## Multiple Sequence Alignment
As mentioned earlier, Multiple Sequence Alignment is the alignment of more than 2 biological sequences.  
Tools for MSA include:
* Clustal W
* Clustal Omega
* DNASTAR
* GLProbs
* MAFFT
* MUSCLE
* T-Coffee
* DECIPHER
* Geneious
