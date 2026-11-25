Overview

This repository contains custom Python and shell scripts used for the construction of copy number variation regions (CNVRs) from whole-genome sequencing data.

Methodology

Deletion and duplication CNVs were processed separately. Duplicate CNV records were removed, and overlapping CNVs were identified using BEDTools with a 75% reciprocal-overlap threshold. The resulting overlap relationships were used to construct connected components using NetworkX. Each connected component was assigned a unique CNVR identifier.

Software Requirements

* Python 3
* NetworkX
* BEDTools

Scripts

The repository contains scripts for:

* Deletion CNVR construction
* Duplication CNVR construction
* Graph-based clustering of overlapping CNV records

Input

The scripts require sorted and formatted BED files containing CNV coordinates and identifiers.

Citation

If you use these scripts in your research, please cite the associated research article and acknowledge the original author.

Contact

For questions regarding the scripts, please contact the corresponding author.
