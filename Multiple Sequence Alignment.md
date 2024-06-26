# Multiple Sequence Alignment of c-Fos protein from different organisms: Human 🕺, Chicken 🐔, Hamster 🐹, Mouse 🐭, Pig 🐖, Carp, Pufferfish 🐡.
## Introduction
c-Fos is a protein that functions as a transcription factor, encoded by the FOS gene in humans. It is part of the Fos family of proteins and forms a heterodimer with Jun proteins to create the activator protein-1 (AP-1) complex. This complex binds to specific DNA sequences to regulate the expression of genes involved in cell proliferation, differentiation, and survival.  
  
As an immediate-early gene, c-Fos is rapidly induced in response to various stimuli, playing a crucial role in signal transduction pathways, cell cycle regulation, and neuronal activity. Its abnormal expression is associated with oncogenesis, making it significant in cancer research and other cellular processes.
## Steps
* Log into the EMBL-EBI [website](http://www.ebi.ac.uk/Tools/msa/clustalo/) and search for **Clustal Omega** at the "service" icon.
  - **N.B**: The User interface may change when you use it, but you should still be able to relatively navigate the website easily.
* Choose the sequence type: Protein, DNA, RNA. In this, case, though, it's going to be Protein.
* Paste the sequences in the space provided. These sequences are often in FASTA format. For this project, the sequences are:

```
  >FOS_CHICKEN Proto-oncogene protein c-fos (Cellular oncogene
fos).
MMYQGFAGEYEAPSSRCSSASPAGDSLTYYPSPADSFSSMGSPVNSQDFCTDLAVSSANF
VPTVTAISTSPDLQWLVQPTLISSVAPSQNRGHPYGVPAPAPPAAYSRPAVLKAPGGRGQ
SIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEEEKSALQA
EIANLLKEKEKLEFILAAHRPACKMPEELRFSEELAAATALDLGAPSPAAAEEAFALPLM
TEAPPAVPPKEPSGSGLELKAEPFDELLFSAGPREASRSVPDMDLPGASSFYASDWEPLG
AGSGGELEPLCTPVVTCTPCPSTYTSTFVFTYPEADAFPSCAAAHRKGSSSNEPSSDSLS
SPTLLAL
>FOS_CARP Proto-oncogene protein c-fos (Cellular oncogene fos).
MMFTSLNADCDASSRCSTASAAAESVACYPLNQTQKFTELSVSSASFVPTVTAISSCPDL
QWMVQPMVSSVAPSNGGARSYNPNPYPKMRVTGTKSPNSNKRARAEQLSPEEEEKKRVRR
ERNKMAAAKCRNRRRELTDTLQAETDELEDEKSALQNDIANLLKEKERLEFILAAHKPIC
KIPSSSVSPIPAASVPEIHSITTSVVSTANAPVTTSSSSSLFSSTASTDSFGSTVEISDL
EPTLEESLELLAKAELETARSVPDVDLSSSLYARDWESLYTPANNDLEPLCTPVVTRTPA
CTTYTSSFTFTYPENDVFPSCGPVHRRGSSSNDQSSDSLNSPTLLTL
>FOS_HUMAN Proto-oncogene protein c-fos (Cellular oncogene fos)
(G0/G1 switch regulatory protein 7).
MMFSGFNADYEASSSRCSSASPAGDSLSYYHSPADSFSSMGSPVNAQDFCTDLAVSSANF
IPTVTAISTSPDLQWLVQPALVSSVAPSQTRAPHPFGVPAPSAGAYSRAGVVKTMTGGRA
QSIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEDEKSALQ
TEIANLLKEKEKLEFILAAHRPACKIPDDLGFPEEMSVASLDLTGGLPEVATPESEEAFT
LPLLNDPEPKPSVEPVKSISSMELKTEPFDDFLFPASSRPSGSETARSVPDMDLSGSFYA
ADWEPLHSGSLGMGPMATELEPLCTPVVTCTPSCTAYTSSFVFTYPEADSFPSCAAAHRK
GSSSNEPSSDSLSSPTLLAL
>FOS_HAMSTER Proto-oncogene protein c-fos (Cellular oncogene
fos).
MMFSGFNADYEASSSRCSSASPAGDSLSYYHSPADSFSSMGSPVNAQDFCTDLSVSSANF
IPTVTAISTSPDLQWLVQPTLVSSVAPSQTRAPHPYGVPTPSTGAYSRAGMVKTVSGGRA
QSIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEDEKSALQ
TEIANLLKEKEKLEFILAAHRPACKIPDDLGFPEEMFVASLDLTGGLPEATTPESEEAFS
LPLLNDPEPKPSLEPVKSISNVELKAEPFDDFLFPASSRPSGSETTARSVPDMDLSGSFY
AADWEPLHSSSLGMGPMVTELEPLCTPVVTCTPSCTTYTSSFVFTYPEADSFPSCAAAHR
KGSSSNEPSSDSLSSPTLLAL
>FOS_MOUSE Proto-oncogene protein c-fos (Cellular oncogene fos).
MMFSGFNADYEASSSRCSSASPAGDSLSYYHSPADSFSSMGSPVNTQDFCADLSVSSANF
IPTVTAISTSPDLQWLVQPTLVSSVAPSQTRAPHPYGLPTQSAGAYARAGMVKTVSGGRA
QSIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEDEKSALQ
TEIANLLKEKEKLEFILAAHRPACKIPDDLGFPEEMSVASLDLTGGLPEASTPESEEAFT
LPLLNDPEPKPSLEPVKSISNVELKAEPFDDFLFPASSRPSGSETSRSVPDVDLSGSFYA
ADWEPLHSNSLGMGPMVTELEPLCTPVVTCTPGCTTYTSSFVFTYPEADSFPSCAAAHRK
GSSSNEPSSDSLSSPTLLAL
>FOS_PIG Proto-oncogene protein c-fos (Cellular oncogene fos).
MMFSGFNADYEASSSRCSSASPAGDSLSYYHSPADSFSSMGSPVNAQDFCTDLAVSSVNF
IPTVTAISISPDLQWLVQPTLVSSVAPSQTRAPHPYGVPTPSAGAYSRAGAVKTMPGGRA
QSIGRRGKVEQLSPEEEEKRRIRRERNKMAAAKCRNRRRELTDTLQAETDQLEDEKSALQ
TEIANLLKEKEKLEFILAAHRPACKIPDDLGFPEEMSVASLDLSGGLPEAATPESEEAFT
LPLLNDPEPKPSVEPVKKVSSMELKAEPFDDFLFPASSRPGGSETARSVPDMDLSGSFYA
ADWEPLHGGSLGMGPMATELEPLCTPVVTCTPSCTAYTSSFVFTYPEADSFPSCAAAHRK
GSSSNEPSSDSLSSPTLLAL
>FOS_PUFFERFISH Proto-oncogene protein c-fos (Cellular oncogene
fos).
MMFTSFNAECDSSSRCSASPVGDNLYYPSPAGSYSSMGSPQSQDFTDLTASSASFIPTVT
AISTSPDLQWMVQPLISSVAPSHRAHPYSPSPSYKRTVMRSAASKAHGKRSRVEQTTPEE
EEKKRIRRERNKQAAAKCRNRRRELTDTLQAETDQLEDEKSSLQNDIANLLKEKERLEFI
LAAHQPICKIPSQMDTDFSVVSMSPVHACLSTTVSTQLQTSIPEATTVTSSHSTFTSTSN
SIFSGSSDSLLSTATVSNSVVKMTDLDSSVLEESLDLLAKTEAETARSVPDVNLSNSLFA
AQDWEPLHATISSSDFEPLCTPVVTCTPACTTLTSSFVFTFPEAETFPTCGVAHRRRSNS
```
* Under the formating options, choose the "ClustalW with Character counts" to get result of alignment format with numbering.
* Other formatting parameters:

| Output Guide tree | Distance Matrix | Dealign Input | MBED-Like Clustering GT | MBED-like Clustering I | Combined I | Order |  
|-------------------|-----------------|---------------|-------------------------|------------------------|------------|-------|  
|        Yes        |        No       |       No      |             Yes         |            Yes         | default(0) |aligned|

 
* Run the test
* Things to note:
  - **Always remember to put the greater than ">" sign at the front of the title of your sequence (which is the first line)**
## Results
On the output page, there are several options to navigate, including downloading your results.

**Pictoral Results of the Output**  

![Screenshot (403)](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/eca3eeaa-712d-4915-9db5-bef879008a9b)
![Screenshot (404)](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/662067c2-bf86-4d80-8a07-65fb0e42272d)
![Screenshot (405)](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/bf17ee63-9162-457b-b44b-8f786cc660f6)
![Screenshot (406)](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/448389ef-0da9-45f8-ae4f-554f53b5db63)  

**Percent Identity Matrix**  

![Screenshot (407)](https://github.com/Onaho-Pascal/Bioinformatics-Projects/assets/156159318/00d8fa27-4434-424c-ba23-e583e3b994e2)  

**Sorry, I had to write the organisms manually on the results so people can easily understand the matching going on 😿**



## Discussion
Observing the colourful pictoral result of the multiple alignment, one can see the different signs (often called consensus signs) beneath each column. These signs tell the level of sequence conservation in that area:  
* An asterisk "*" is for columns in which all the amino acids are identical.
* A colon ":" is for highly conserved columns showing similar amino acids.
* A dot "." is for partially conserved columns with lesser similar amino acids.
* No symbol means the column is not conserved at all.

An area with a lot of asterisks and colons means a highly conserved motif, meanwhile an area with a lot of inexistent symbols or an area with a lot of gaps represents non-conserved regions.  

For the percent identity matrix, there are a number of shared conservation among species:  
* Humans and Pigs share a close conservation of the c-Fos protein at 96.32%
* Humans and Hamster also share a close conservation of the c-Fos protein at 94.26%
* Pigs and Hamster share at 94.47%
* Humans and Mouse share at 93.86%

The degree to which the organisms share amino acid sequence are as follows:  
* Human: Pig > Hamster > Mouse >> Chicken >>> Puffer-fish >>> Carp.
* Pig: Human > Hamster > Mouse >> Chicken >>> Puffer-fish >>> Carp.
* Hamster: Mouse > Pig > Human >> Chicken >>> Puffer-fish >>> Carp.
* Mouse: Hamster > Human > Pig >> Chicken >>> Puffer-fish >>> Carp.
* Carp: Puffer-fish >>> Hamster >>> Mouse >>> Human >>> Pig >>> Chicken.
* Puffer-fish: Carp >>> Hamster >>> Mouse >>> Human >>> PIg >>> Chicken.

Multiple sequence has its different uses. Aligning multiple sequences can help to identify the conserved motifs  which are functionally important, just as we have seen in this result (the conserved motifs or regions). Further analysis could even give insights to the active binding sites and critical sites for protein function.  

Additionally, assuming we knew the c-Fos protein structure of a pig, it won't be difficult to infere the structure of a human, since the share conservative motif or region is high between both species.

## Conclusion
By revealing conserved and variable regions across multiple sequences, MSA is quite important for understanding the functional, structural, and evolutionary aspects of biological molecules.  

**Potential applications of this result involves**
* Phylogenetic Analysis: evolutionary relationships and phylogenetic trees could be conducted from this result
* Structural Prediction: Like I mentioned in the last part of the discussion, if one of the species' c-Fos protein is not known, this result can effectively aid the prediction of the unknown protein structure, especially for species with highyl conserved region or motif.
* Target Selection: This result can help in selecting target regions for further experimental studies, such as mutagenesis or functional assays.

# Multiple Sequence Alignment of the Vascular Endothelial Growth Factor A proteins from different Organisms: Bovine🐮, Chick🐤, Horse🐴, Human🧍‍♀️, Hamster🐹, Mouse🐁, Pig🐖.
## To be updated!!! 😿


