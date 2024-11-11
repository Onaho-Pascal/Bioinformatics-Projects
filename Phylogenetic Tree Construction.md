# Phylogenetic Tree Construction of c-Fos protein from different organisms: Human 🕺, Chicken 🐔, Hamster 🐹, Mouse 🐭, Pig 🐖, Carp, Pufferfish 🐡. 

## Steps carried out for this tree construction
1. Set the working directory, installed, and loaded the necessary packages.
2. Loaded the protein sequence data of the different organisms into R.
3. Aligned the protein sequences.
4. Computed the distance matrix.
5. Constructed the phylogenetic tree.

 ## Important codes 
Loaded sequences using readAAStringSet().
Aligned sequences with msa().
Calculated the distance matrix with dist.ml().
Built the tree using either nj() for NJ.
Plotted the resulting tree. 
```
install.packages(c("ape", "seqinr", "phangorn"))
BiocManager::install("msa")

library(Biostrings)
library(ape)
library(seqinr)
library(phangorn)
library(msa)
# Replace "your_protein_sequences.txt" with the path to your file
protein_sequences <- readAAStringSet("Ms.txt", format = "fasta")

# Multiple sequence alignment
alignment <- msa(protein_sequences, method = "ClustalW")
alignment_phylo <- as.phyDat(alignment, type = "AA")

# Computing the distance matrix
dist_matrix <- dist.ml(alignment_phylo, model = "JTT")
# Tree construction
tree_nj <- nj(dist_matrix)
plot(tree_nj, main = "Neighbor-Joining Phylogenetic Tree")
```
![Rplot24](https://github.com/user-attachments/assets/ea8bff62-6061-4590-8e70-a54fd611f32b)

 

## Result Interpretation

**Pairwise Observations:**
Pig - Human: The c-Fos sequences for pig and human show close similarity, clustering together as the first pair. This pairing aligns with established mammalian phylogeny, where humans and pigs share a closer evolutionary relationship compared to more distantly related species like fish or birds. The similarity in c-Fos sequences indicates conserved functional roles in cell signaling and gene regulation, common to these mammals.

Mouse - Hamster: Another clear clustering appears between mouse and hamster, which are both rodents. This pair further reflects the evolutionary closeness within Rodentia. Their shared evolutionary branch in the tree reinforces the idea of similar physiological and genetic mechanisms governing c-Fos functionality among rodents.

Carp - Pufferfish: In this pair, the c-Fos sequences from carp and pufferfish are grouped together, suggesting an evolutionary similarity in fish species, despite their divergence in other ecological and physical characteristics. This pairing illustrates the degree of conservation within fish, where c-Fos plays a similar functional role, perhaps related to aquatic adaptations and species-specific developmental pathways.

**Hierarchical Clustering:**
Chicken - (Carp - Pufferfish): The next branch places the chicken closer to the carp and pufferfish than to any of the mammals. This configuration is consistent with evolutionary theory, where birds and fish represent more basal lineages relative to mammals. Chickens share a more ancient common ancestor with fish species than with the mammalian cluster. The moderate sequence similarity here likely reflects functional aspects of c-Fos that have been conserved across these vertebrate lineages but diverged as the mammalian lineage evolved.

(Mouse - Hamster) - (Human - Pig): The tree further reveals a distinction between the rodents (mouse and hamster) and the larger mammals (human and pig), grouping these two pairs together. This clustering reflects shared evolutionary history within mammals, with rodent and non-rodent mammals branching off at different points but still sharing closer ancestry compared to birds and fish. The distinction of these groups highlights mammalian-specific evolutionary pressures and adaptations in c-Fos protein function.

**Overall Hierarchical Structure:**
The highest-level grouping in the tree can be described as: (((Mouse - Hamster) - (Human - Pig)) - (Chicken - (Carp - Pufferfish)))

This structure suggests a deep evolutionary divergence between mammals and non-mammals. Within mammals, rodents (mouse and hamster) diverged earlier from the lineage leading to non-rodent mammals (human and pig). The placement of chicken as an intermediary between mammals and fish indicates that birds are evolutionarily closer to mammals than fish, consistent with vertebrate phylogeny.

**Conclusion**
The phylogenetic tree for c-Fos across these organisms not only confirms known evolutionary relationships but also highlights the conservation of this critical protein across species. The distinct clusters (mammals, birds, and fish) reflect the evolutionary pressures that shaped the c-Fos protein’s structure and function in various organisms. This phylogenetic analysis underscores the importance of c-Fos in evolutionary biology and functional genomics, helping us better understand gene conservation, adaptation, and divergence across the animal kingdom.
## Importance of Phylogenetic Tree Construction

**Understanding Evolutionary Relationships**
Phylogenetic trees help illustrate how species or genes are related over evolutionary time. By tracing back branches, researchers can determine common ancestors, lineage divergence, and the order of evolutionary events.

**Taxonomy and Classification**
Phylogenetics provides a framework for the classification of organisms, helping refine taxonomy by identifying evolutionary relationships. This often leads to the reclassification of organisms based on genetic evidence rather than purely physical characteristics.  

**Studying Pathogen Evolution and Spread**
In microbiology and epidemiology, phylogenetic trees are used to study the evolution and transmission pathways of viruses, bacteria, and other pathogens. For example, phylogenetic trees were crucial in tracing the evolution and spread of viruses like HIV, SARS-CoV-2, and influenza.  

**Drug and Vaccine Development**
Phylogenetics assists in identifying conserved regions in pathogenic genomes, which can serve as targets for drugs and vaccines. Understanding evolutionary pressures and patterns helps in designing treatments that are effective across various strains or even preemptive to mutations.  

**Gene Family and Protein Function Studies**
In molecular biology, constructing phylogenetic trees of gene families helps reveal functional relationships between genes. By understanding how certain genes evolved, researchers can infer functional similarities, which aids in predicting protein functions for newly discovered or uncharacterized genes.
