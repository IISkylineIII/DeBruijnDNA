### De Bruijn Sequence Generator for DNA k-mers

This Python script generates a De Bruijn sequence for a given alphabet size and subsequence length, tailored for DNA applications using the nucleotides A, C, G, and T.

A De Bruijn sequence of order n over an alphabet of k symbols is a cyclic sequence in which every possible substring of length n appears exactly once. These sequences are widely used in bioinformatics, particularly in genome assembly and k-mer analysis.

### Features
Generates a minimal cyclic sequence that includes every possible k-mer exactly once.

Customizable alphabet size and k-mer length.

Default alphabet: "ACGT" (DNA bases).

### Usage
from itertools import product

def de_bruijn_sequence(k, n):
    # Function body...
    
# Example: Generate a 4-universal string (all 4-mers over ACGT)
result = de_bruijn_sequence(4, 4)
print(result)

### Parameters
k: Size of the alphabet. Default is 4 for DNA (A, C, G, T).

n: Length of the k-mers you want the sequence to include.

### Output
A string of length k^n + n - 1 representing the De Bruijn sequence.

### Example 
Input: k = 4, n = 4
Output: AAAAACAAAGAAATAACACCACGACTAGAGCAGGAGTAGTATCATCCCGCCTCGCTG...

### Applications
Genome assembly using de Bruijn graphs.

Testing DNA synthesis tools with comprehensive k-mer coverage.

Efficient storage and analysis of k-mers in bioinformatics.
