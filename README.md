# transcriptx

A pipeline for autommated annotation of whole-transcriptome shotgun assemblies that integrates:

- Open Reading Frame detection with TransDecode (http://transdecoder.github.io/)
- Identification of tRNA genes with tRNAscan-SE (http://lowelab.ucsc.edu/tRNAscan-SE/).
- Identification of rRNA genes with identification with RNAmmer (www.cbs.dtu.dk/services/RNAmmer/).
- Identification of other families of ncRNAs with Infernal (http://eddylab.org/infernal/) and Rfam (rfam.sanger.ac.uk/).
- Secondary structure prediction with RNAfold (http://rna.tbi.univie.ac.at/).
- CD-HIT database clustering (http://weizhongli-lab.org/cd-hit/)
- Protein annotation with BLASTx (https://blast.ncbi.nlm.nih.gov/) vs. Uniprot (http://www.uniprot.org/).
- Protein family annotation with Pfam (http://pfam.xfam.org/) by HMMER (http://hmmer.janelia.org/).
- Signal peptide identification in proteins with SignalP (http://www.cbs.dtu.dk/services/SignalP/).
- Transmembrane-helix identification with TMHMM (http://www.cbs.dtu.dk/services/TMHMM/).


Installation
-

`$ -xvfz transcriptx.tar.gz`

`$ cd transcriptx`

`$ sudo python install.py`

As RNAmmer, SignalP and TMHMM are not distributed are only avaliable under academic or comercial license, they are not provided along with transcriptx, and must be obtained from their respective repositories. After downloading, decompressing and installing, you can add then to the transcriptix pipeline using the following commands:

`$ transcriptx.py --add_rnammer RNAMMER_DIR_PATH`

`$ transcriptx.py --add_signalp SIGNALP_DIR_PATH`

`$ transcriptx.py --add_tmhmm TMHMM_DIR_PATH`

Running
-

`transcriptx.py --protein_db proteins.fasta --transcriptome assembly.fasta --out_dir resultado --threads 4`


