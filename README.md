﻿# MAnorm
[![travis-ci](https://travis-ci.org/shao-lab/MAnorm.svg?branch=master)](https://travis-ci.org/shao-lab/MAnorm)
[![Documentation Status](https://readthedocs.org/projects/manorm/badge/?version=latest)](http://manorm.readthedocs.io/en/latest/?badge=latest)
[![pypi](https://img.shields.io/pypi/v/MAnorm.svg)](https://pypi.python.org/pypi/MAnorm)
[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat-square)](http://bioconda.github.io/recipes/manorm/README.html)
[![license](https://img.shields.io/pypi/l/MAnorm.svg)](https://github.com/shao-lab/MAnorm/blob/master/LICENSE)

## Introduction

ChIP-Seq is widely used to characterize genome-wide binding patterns of transcription factors and other chromatin-associated proteins. Although comparison of ChIP-Seq data sets is critical for understanding cell type-dependent and cell state-specific binding, and thus the study of cell-specific gene regulation, few quantitative approaches have been developed.

Here, we present a simple and effective method, MAnorm, for quantitative comparison of ChIP-Seq data sets describing transcription factor binding sites and epigenetic modifications. The quantitative binding differences inferred by MAnorm showed strong correlation with both the changes in expression of target genes and the binding of cell type-specific regulators.

## Citation

> [MAnorm: a robust model for quantitative comparison of ChIP-Seq data sets.](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2012-13-3-r16) Shao Z, Zhang Y, Yuan GC, Orkin SH, Waxman DJ.   *Genome Biol. Mar 16;13(3):R16.*


## Documentation

To see the full documentation of MAnorm, please refer to:

http://manorm.readthedocs.io/en/latest/ 

## Installation

The latest version release of MAnorm is available at [PyPI](https://pypi.python.org/pypi/MAnorm): 
```
pip install manorm
```
Or you can install MAnorm via conda:

```
conda install -c bioconda manorm
```

MAnorm uses [setuptools](https://setuptools.readthedocs.io/en/latest/) for installation from source code. 
The source code of MAnorm is hosted on GitHub: https://github.com/shao-lab/MAnorm

You can clone the repo and execute the following command under source directory: 
```
python setup.py install
```

## Usage
manorm [-h] [-v] --p1 peaks_file1 --p2 peaks_file2 --r1 reads_file1 --r2 reads_file2 -o output_name

Example: 
```
manorm --p1 sample1_peaks.bed --p2 sample2_peaks.bed --r1 sample1_reads.bed --r2 sample2_reads.bed -o sample1_vs_sample2
```

**Note:** Using -h/--help for the details of all arguments.

  
## License

[BSD 3-Clause License](https://github.com/shao-lab/MAnorm/blob/master/LICENSE)
