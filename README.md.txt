Forced Alignment Using Montreal Forced Aligner (MFA)
This repository contains all materials for the Forced Alignment assignment using MFA for speech audio and transcript alignment.

Contents
Report.pdf : Final report containing analysis, tables, and screenshots.

aligned_output/ : Folder with MFA-generated TextGrid files (aligned phoneme and word boundaries).

data/ (optional) : Audio (.wav) and transcript (.txt) files used for alignment.

colab_notebook.ipynb (optional) : Google Colab notebook with all installation and alignment commands.

Setup Instructions
Install Praat for visualizing TextGrid annotations.

Mount Google Drive in Colab or clone this repository on your local machine.

If running alignments, install MFA via conda:

text
conda install -c conda-forge montreal-forced-aligner
Download pretrained MFA models:

text
mfa model download acoustic english_us_arpa
mfa model download dictionary english_us_arpa
Run forced alignment:

text
mfa align data/wav data/transcripts english_us_arpa english_us_arpa aligned_output
How to Use
Use Praat to open a .wav file and its corresponding .TextGrid file for detailed phoneme and word boundary visualization.

Refer to the report for a detailed analysis of the alignment results.

Notes
Ensure consistency in file naming between audio and transcript files.

Output TextGrid files are located in aligned_output/.

Contact
For questions or feedback, please contact V John Joe at v.john@op.iitg.ac.in .

