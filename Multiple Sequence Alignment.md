# Multiple Sequence Alignment of c-Fos protein from different organisms: Human 🕺, Chicken 🐔, Hamster 🐹, Mouse 🐭, Pig 🐖, Carp, Pufferfish 🐡.
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

## Conclusion
