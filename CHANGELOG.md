# nf-core/hic: Changelog

## v1.1.0 - 2019-10-15

* Support 'N' base motif in restriction/ligation sites
* Support multiple restriction enzymes/ligattion sites (comma separated) ([#31](https://github.com/nf-core/hic/issues/31))
* Add --saveInteractionBAM option
* Add DOI ([#29](https://github.com/nf-core/hic/issues/29))
* Fix bug for reads extension _1/_2 ([#30](https://github.com/nf-core/hic/issues/30))
* Update manual ([#28](https://github.com/nf-core/hic/issues/28))

## v1.0 - 2019-05-06

First version of nf-core Hi-C pipeline which is a Nextflow implementation of
the [HiC-Pro pipeline](https://github.com/nservant/HiC-Pro/).
Note that all HiC-Pro functionalities are not yet all implemented.
The current version supports most protocols including Hi-C, in situ Hi-C,
DNase Hi-C, Micro-C, capture-C or HiChip data.

In summary, this version allows :

* Automatic detection and generation of annotation files based on igenomes
if not provided.
* Two-steps alignment of raw sequencing reads
* Reads filtering and detection of valid interaction products
* Generation of raw contact matrices for a set of resolutions
* Normalization of the contact maps using the ICE algorithm
* Generation of cooler file for visualization on [higlass](https://higlass.io/)
* Quality report based on HiC-Pro MultiQC module
