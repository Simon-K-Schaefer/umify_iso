# umify_iso
Script for UMI error correction

Dependencies: Perl5

PCR and sequencing errors are corrected by UMI pattern matching and selecting reads containing valid UMIs. Reads with matching UMIs are corrected to the most abundant read per UMI. To exclude quantitative bias introduced during Multiplex PCR reads are normalized to unique mRNA sequences. Reads shorter than 50 nucleotides are filtered for additional quality control.

## Installation

Download the archive, decompress and copy the script to folder with input data.

https://github.com/Simon-K-Schaefer/umify_iso/archive/refs/heads/main.zip



## command line usage

Please note the script only works for samples created with primers as described here:
"method paper pending"


>perl umify_normalized_iso.pl sample.fasta


Output: The script creates a folder containing a log file with primer and UMI information as well as new fasta files with corrected sequences for all reads and primer defined isotypes.






## Citing umify

Copyright (c) 2021, Simon Schaefer
All rights reserved.

This source code is licensed under the BSD-style license found in the
LICENSE file in the root directory of this source tree. 

If you are using umify in any published work, please cite:

Werner A, Schäfer S, Gleußner N, Nimmerjahn F, Winkler TH. Determining immunoglobulin-specific B cell receptor repertoire of murine splenocytes by next-generation sequencing. STAR Protoc. 2022 Apr 9;3(2):101277. doi: 10.1016/j.xpro.2022.101277. PMID: 35434659; PMCID: PMC9010798.
