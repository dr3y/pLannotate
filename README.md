[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Python 3](https://img.shields.io/badge/Language-Python_3-steelblue.svg)

<img width="400" alt="pLannotate_logo" src="images/pLannotate.png">

Online Annotation
=================

pLannotate is web server for automatically annotating engineered plasmids.

Please visit http://plannotate.barricklab.org/


Local Installation
==================

If you wish you to use pLannotate as a local server, enter the following commands on your terminal (requires [Conda](https://docs.conda.io/en/latest/)).

Clone the repository onto your computer:
```
git clone https://github.com/barricklab/pLannotate
```
Move into the repository:
```
cd pLannotate/
```
Unzip the compressed database files:
```
gunzip ./BLAST_dbs_gz/*
```
Rename the directory containing the now uncompressed files:
```
mv ./BLAST_dbs_gz/ ./BLAST_dbs
```
Create the Conda environment:
```
conda env create -f environment.yml
```
Activate the Conda environment:
```
conda activate pLannotate
```
Launch pLannotate:
```
streamlit run pLannotate_app.py
```

After execution of the final command, pLannotate should launch in your default web browser, or you may simply navigate to http://localhost:8501 in your web browser.

About
=====
pLannotate is currently developed by [Matt McGuffie](https://twitter.com/matt_mcguffie) at the [Barrick lab](https://barricklab.org/twiki/bin/view/Lab), University of Texas at Austin, Austin, Texas.