# Pairwise Alignment of c-fos Protein and ATF3 Protein.
## Introduction
Pairwise Sequence Alignment is a type of sequence alignment used to identify similar regions that may indicate relationships between two biological sequences. This relationship could be functional, structural, evolutionary, or a combination of two or more of these relationships.
Alignment can either be Global or Local. Global alignment matches the entire length of the sequences, while Local alignment looks for sub-sequences of both sequences and matches them optimally to each other.  
  
  The **c-Fos** protein is a proto-oncogene homologous to the retroviral oncogene: v-Fos, and It was first discovered in rat fibroblasts.
The c-fos protein is a cell cycle controller at the G0/G1 checkpoint. 
It plays an important role in many cellular functions and has been found to be over expressed in a variety of cancers.  
  
  The **ATF3** Protein is also called the Activating transcription factor 3 protein and is a part of the mammalian activation transcription factor/cAMP responsive element-binding (CREB) protein family of transcription factors.

## Global Alignment of c-Fos and ATF3
Using the EMBOSS Needle tool, the sequences of both proteins were Globally aligned. 
Steps include:  
* Access the EMBOSS Needle tool from the website: https://www.ebi.ac.uk/jdispatcher/psa/emboss_needle
* Since the alignment is for Protein sequences, leave the Protein option ticked.
* Paste or upload the sequences of the protein to be aligned and the sequences should be uploaded in FASTA FORMAT  
  FASTA Format for c-Fos Protein:   
  uniprot|P01100|FOS_HUMAN Proto-oncogene c-Fos;
MMFSGFNADYEASSSRCSSASPAGDSLSYYHSPADSFSSMGSPVNAQDFCTDLAVSSANF
IPTVTAISTSPDLQWLVQPALVSSVAPSQTRAPHPFGVPAPSAGAYSRAGVVKTMTGGRA
QSIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEDEKSALQ
TEIANLLKEKEKLEFILAAHRPACKIPDDLGFPEEMSVASLDLTGGLPEVATPESEEAFT
LPLLNDPEPKPSVEPVKSISSMELKTEPFDDFLFPASSRPSGSETARSVPDMDLSGSFYA
ADWEPLHSGSLGMGPMATELEPLCTPVVTCTPSCTAYTSSFVFTYPEADSFPSCAAAHRK
GSSSNEPSSDSLSSPTLLAL  

FASTA Format for ATF3 Protein:  

  uniprot|P18847|ATF3_HUMAN Cyclic AMP-dependent transcription factor ATF-3;
MMLQHPGQVSASEVSASAIVPCLSPPGSLVFEDFANLTPFVKEELRFAIQNKHLCHRMSS
ALESVTVSDRPLGVSITKAEVAPEEDERKKRRRERNKIAAAKCRNKKKEKTECLQKESEK
LESVNAELKAQIEELKNEKQHLIYMLNLHRPTCIVRAQNGRTPEDERNLFIQQIKEGTLQ
S

**BE SURE TO PLACE A GREATER THAN SIGN DIRECTLY IN FRONT OF BOTH FASTA FORMAT FILES AFTER COPY AND PASTING BEFORE YOU RUN THE ALIGNMENT!!!** 
 
 * Set certain parameters before running the sequence alignment  
 Parameters used include:  
 Matrix: EPAM100  
 Gap Open: 10  
 Gap Extended: 0.5  
 End Gap: False  
 End Gap Open: 10  
 End Gap Extend: 0.5  
 Output Format: pair  
 Sequence Type: Protein
* Global Alignment using PAM 100:
![Snapshot of the result using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/80496bff-e43f-479b-8986-f8067bc07c2f)
* Global Alignment using PAM 200:
![Snapshot of the result using PAM 200](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/9c852c6f-3bcb-4e95-a655-52324f4a192f)

## Results and Interpretation for the Global Alignment 
| Sub Matrix | Length | Identity | Similarity | Gaps | Score |
|------------|--------|----------|------------|------|-------|
|  PAM 100   |   402  |68/402 (16.9%)| 112/402 (27.9%) | 243/402 (60.4%) | 218.5 |
|  PAM 200   |   403  |63/403 (15.6%)| 120/403 (29.8%) | 245/403 (60.4%) | 294.5 |  

As can be viewed from the images, the FOS protein appears at the upper line, while the ATF protein appears at the lower line. The alignment is too long to be presented in a single line, hence, it breakage into segments. The numbers that appear at the right side in the last segment represents the location of the last amino acids at each sequence and therefore, represents the sequence length. There are certain things to take note of:
* A gap in the alignment is represented by a hyphen.
* Identity is represented with a solid line.
* High similarity is represented with two dots.
* Low or no similarity is represented with one dot.
* A good alignment is expected to include a large area with lot of lines and lot of two dots. i.e. An area with high identity and similarity.
* The length as shown in the upper part of the image or the table presented above, is higher than the normal sequence length of the protein, and this is because gaps were also included in the count.
* Percentage of identity is the number of identical amino acids divided by the alignment length.
* Percentage of similarity is the number of similar amino acids divided by the alignment length.
* Percentage of similarity is the number of gaps divided by the alignment length.  
When the substitution matrix is changed, the results change depending on size of the matrix. A higher matrix number the greater the evolutionary distance and therefore, a higher similarity than when a lower matrix number. Also, more gaps are introduced when a higher matrix is used.
## Local Alignment of c-Fos and ATF3 
Using the EMBOSS Needle tool, the sequences of both proteins were locally aligned. 
Steps include:
* Access the EMBOSS Water tool from the website: https://www.ebi.ac.uk/jdispatcher/psa/emboss_water
* Since the alignment is for Protein sequences, leave the Protein option ticked.
* Paste or upload the sequences of the protein to be aligned and the sequences should be uploaded in FASTA FORMAT, using the FASTA Format sequences provided above.
* **DO NOT FORGET THE GREATER THAN SIGN**
* Local Alignment using PAM 100:
  ![Snapshot of Local Alignment using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/3a3ab95f-4cf6-4f83-9769-71a9a28ffe91)
  
* Local Alignment using PAM 200:
 ![Snapshot of the Local Alignment result using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/b3e5d117-413a-4cb1-9c3f-1254ca5ae0c6)

## Results and Intepretation for the Local Alignment
| Sub Matrix | Length | Identity | Similarity | Gaps | Score |
|------------|--------|----------|------------|------|-------|
|  PAM 100   |  200   | 59/200 (29.5%) | 94/200 (47.0%) | 69/200 (34.5%) | 224.5 |
|  PAM 200   |  245   | 63/245 (25.7%) | 120/245 (49.0%) | 88/245 (35.9%) | 298.5 |  

Explanation given for the Global alignment is almost entirely applicable to the Local alignment. This includes the difference in results when substitution matrix numbers are changed i.e An increase in substitution matrix number will lead to a decrease ⬇️ in identical percentage and an increase ⬆️ in similarity percentage.  
Naturally, it is expected that the length of sequence from a local alignment result would be shorter than from a global alignment result of the same sequence. This is because local alignment only aligns a local area of the sequence most similar, while the global aligns the whole sequence.

## Conclusion
How do we know when to use Global or Local alignment? OR what matrix parameters to use?  
I've learnt that there is no one way to know and it all depends on the expreience of the bioinformatics scientist performing the sequence alignment and what is needed. Usually, Global alignments are performed on homologous genes and proteins, while local alignments are performed on non-homologous genes or proteins to find the most similar sections or domains of their sequences.  
In this alignment, both proteins seems have a strong region of similarity and identity at position 137 to 188 for c-FOS protein and position 86 to 137 for ATF3 protein in both the Local and Global sequences. 
