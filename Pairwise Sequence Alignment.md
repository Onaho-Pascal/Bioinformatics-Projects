# Pairwise Alignment of c-fos Protein and ATF3 Protein.
## Introduction
The c-Fos protein is a proto-oncogene homologous to the retroviral oncogene: v-Fos, and It was first discovered in rat fibroblasts.
The c-fos protein is a cell cycle controller at the G0/G1 checkpoint. 
It plays an important role in many cellular functions and has been found to be over expressed in a variety of cancers.
The ATF3 Protein is also called the Activating transcription factor 3 protein and is a part of the mammalian activation transcription factor/cAMP responsive element-binding (CREB) protein family of transcription factors.

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
![Snapshot of the result using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/80496bff-e43f-479b-8986-f8067bc07c2f)
When PAM is set to 200:
![Snapshot of the result using PAM 200](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/9c852c6f-3bcb-4e95-a655-52324f4a192f)

## Local Alignment of c-Fos and ATF3 
Using the EMBOSS Needle tool, the sequences of both proteins were locally aligned. 
Steps include:
* Access the EMBOSS Water tool from the website: https://www.ebi.ac.uk/jdispatcher/psa/emboss_water
* Since the alignment is for Protein sequences, leave the Protein option ticked.
* Paste or upload the sequences of the protein to be aligned and the sequences should be uploaded in FASTA FORMAT, using the FASTA Format sequences provided above.
* **DO NOT FORGET THE GREATER THAN SIGN**
* Local Alignment using PAM 100
  ![Snapshot of Local Alignment using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/3a3ab95f-4cf6-4f83-9769-71a9a28ffe91)
  
* Local Alignment using PAM 200
 ![Snapshot of the Local Alignment result using PAM 100](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/b3e5d117-413a-4cb1-9c3f-1254ca5ae0c6)

 
