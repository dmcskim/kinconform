# Test script for kinconform
# 
# Example structures are taken from RCSB.org
#

PY = python

all: test

clean: 
	rm -vf *.out pdbs.fasta pdbs.*cma pdbs.*seq

test: ../kinconform 2gs2.pdb 4afj.pdb
	$(PY) $^ --base ../ > test.out

