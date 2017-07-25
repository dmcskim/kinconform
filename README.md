# KinConform -- Kinase conformation classification
[![DOI](https://zenodo.org/badge/69583628.svg)](https://zenodo.org/badge/latestdoi/69583628)
======
Classify kinase structures as active/inactive. 
## Description of methods
------
KinConform takes any number of input structures, separates their chains and generates a fasta file of sequences. This fasta file is aligned (using MAPGAPS) to kinase profiles, identifying which chains are kinases. A series of measurements are then taken for each kinase chain and used as input to a machine learning classifier.

The output is tab-delimited and displays the conformation (active/inactive) for each input kinase chain.
## Usage
------
./kinconform XXX.pdb YYY.pdb ZZZ.pdb > a.out

To run test structures, simply `cd test` and `make all`.

Note: the profile and model directories should be colocated with kinconform. To install, add a symbolic link to kinconform from your bin/ directory.
# Dependencies
------
Please ensure the following software is installed:
- `NumPy <http://www.numpy.org>`
- `MDAnalysis <http://www.mdanalysis.org>`
- `Biocma <https://github.com/etal/biocma>`
- `MAPGAPS <http://mapgaps.igs.umaryland.edu>` 
