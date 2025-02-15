# BibHelioTech

[![DOI](https://zenodo.org/badge/515186537.svg)](https://zenodo.org/badge/latestdoi/515186537)
[![License](https://img.shields.io/github/license/ADablanc/BibHelioTech.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)<br />
![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/ADablanc/BibHelioTech)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/ADablanc/BibHelioTech)<br />
![GitHub repo size](https://img.shields.io/github/repo-size/ADablanc/BibHelioTech)<br />
[![GitHub issues](https://img.shields.io/github/issues/ADablanc/BibHelioTech)](https://github.com/ADablanc/BibHelioTech/issues)

## BibHelioTech project description
BibHelioTech is a program for the recognition of temporal expressions and entities (satellites, instruments, regions) extracted from scientific articles in the field of heliophysics.<br />
It was developed at IRAP (Institut de Recherche en Astrophysique et Planétologie, Toulouse https://www.irap.omp.eu/) in the frame of an internship by A. Dablanc supervised by V. Génot.<br />
Its main purpose is to retrieve events of interest which have been studied and published, and associate them with the full context of the observations. It produces standardized catalogues of events (time intervals, satellites, instruments, regions, metrics) which can then be exploited in space physics visualization tools such as AMDA (http://amda.cdpp.eu/).

## Installation guide
STEP 1: install all dependency<br />
&nbsp;&nbsp;&nbsp;On your shell, run: pip install -r requirements.txt<br />
&nbsp;&nbsp;&nbsp;Don't forget to install SUTime Java dependencies, more details on: https://pypi.org/project/sutime/ <br />
&nbsp;&nbsp;&nbsp;Put the "english.sutime.txt" under sutime install directory, jars/stanford-corenlp-4.0.0-models.jar/edu/stanford/nlp/models/sutime/

STEP 2: tesseract 5.1.0 installation (Ubuntu exemple)<br />
&nbsp;&nbsp;&nbsp;sudo apt update<br />
&nbsp;&nbsp;&nbsp;sudo add-apt-repository ppa:alex-p/tesseract-ocr-devel<br />
&nbsp;&nbsp;&nbsp;sudo apt install -y tesseract-ocr<br />
&nbsp;&nbsp;&nbsp;sudo apt update<br />
&nbsp;&nbsp;&nbsp;tesseract --version

STEP 3: GROBID (0.7.1) installation<br />
&nbsp;&nbsp;&nbsp;install GROBID under ../<br />
&nbsp;&nbsp;&nbsp;Follow install instruction on: https://grobid.readthedocs.io/en/latest/Install-Grobid/ <br />
&nbsp;&nbsp;&nbsp;Make sure you have JVM 8 used by default !

STEP 4: GROBID python client installation<br />
&nbsp;&nbsp;&nbsp;install GROBID python client under ../<br />
&nbsp;&nbsp;&nbsp;Follow install instruction on: https://github.com/kermitt2/grobid_client_python <br />

## User guide
Put Heliophysics articles in pdf format under BibHelio_Tech/DATA/Papers.<br />
You just have to run "MAIN.py".<br />
<br />
optionally if you want to have AMDA catalogues by satellites,<br />
you need to run "SATS_catalogue_generator.py".

## License
If you use or contribute to BibHelio_Tech, you agree to use it or share your contribution following this license.

## Authors
[Axel Dablanc]: axel.alain.dablanc@gmail.com<br />
[Vincent Génot]: vincent.genot@irap.omp.eu
