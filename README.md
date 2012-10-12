GapEst
======

Reference implementation of the scaffolding gap size estimation
algorithm by Kristoffer Sahlin.

Dependencies
------------
Python modules scipy, pysam0.6, networkx1.4

INPUT
-----

Requierd arguments:

1. -c a contig file (path to) 

2.  -f a BAM of SAM file  (path to)

3. -m  the mean of the insert sizes of the library (integer)

4. -s standard deviation of the library (integer)

5. -r (integer number) Mean read length for each of the libraries. 

Optional:
8 -e (integer number) The least amount of witness links that is needed to create a link edge in graph to estimate gap for


Example run
-----------

    python Main.py  -c /path/to/contigfile.fa -f /path/to/file1.bam /path/to/file2.bam -o /path/to/output -m <mean> -s <std dev>
