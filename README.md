# transcriptx

A pipeline for autommated annotation of whole-transcriptome shotgun assemblies. 

- Open Reading Frame detection with TransDecode (http://transdecoder.github.io/)
- Identification of tRNA genes with tRNAscan-SE (http://lowelab.ucsc.edu/tRNAscan-SE/).
- Identification of rRNA genes with identification with RNAmmer (www.cbs.dtu.dk/services/RNAmmer/).
- Identification of other families of ncRNAs with Infernal (http://eddylab.org/infernal/) and Rfam (rfam.sanger.ac.uk/).
- Secondary structure prediction with RNAfold (rna.tbi.univie.ac.at/).
- Protein annotation with BLASTx (https://blast.ncbi.nlm.nih.gov/) vs. Uniprot (http://www.uniprot.org/).
- Protein family annotation with Pfam (http://pfam.xfam.org/) by HMMER (http://hmmer.janelia.org/).
- Signal peptide identification in proteins with SignalP (http://www.cbs.dtu.dk/services/SignalP/).
- Transmembrane-helix identification with TMHMM (http://www.cbs.dtu.dk/services/TMHMM/).
