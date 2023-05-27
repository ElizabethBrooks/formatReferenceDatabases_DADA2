# FormatReferenceDatabases_DADA2
Repository for scripts to format reference databases for DADA2.

BASH script to split the input fasta file and run a separate BASH script to parse CO1_.fasta and CO1_taxonomy.txt and create a fasta file with the sequence ID replaced with the taxonomic assignment (column 2) from CO1_taxonomy.txt

https://benjjneb.github.io/dada2/training.html
https://ucedna.com/reference-databases-for-metabarcoding 

For example, looking at the data for sample "JN275563.1":
Input Files
CO1_.fasta
>JN275563.1
CTATCATCAGGAATTGCTCATGCTGGTGCATCTGTTGACTTAGCTATTTTTTCTTTACATTTAGCGGGGATTTCTTCTATTTTAGGAGCAGTAAATTTTATTACTACTGTAATTAATATACGCTCAGAAGGAATTTCATATGACCGAATACCATTATTTGTTTGATCAGTAATTATTACTGCTATTTTATTATTATTATCATTACCTGTACTAGCAGGTGCAATCACTATACTTCTAACAGACCGAAATTTAAATACTTCATTTTTTGATCCTGCTGGAGGTGGTGACCCCATCCTATACCAACATTTATTC

CO1_taxonomy.txt
JN275563.1 Eukaryota;Arthropoda;Insecta;Diptera;Chironomidae;Smittia;Smittia extrema

Output File
CO1_taxonomyAssignment.fasta
>Eukaryota;Arthropoda;Insecta;Diptera;Chironomidae;Smittia;Smittia
CTATCATCAGGAATTGCTCATGCTGGTGCATCTGTTGACTTAGCTATTTTTTCTTTACATTTAGCGGGGATTTCTTCTATTTTAGGAGCAGTAAATTTTATTACTACTGTAATTAATATACGCTCAGAAGGAATTTCATATGACCGAATACCATTATTTGTTTGATCAGTAATTATTACTGCTATTTTATTATTATTATCATTACCTGTACTAGCAGGTGCAATCACTATACTTCTAACAGACCGAAATTTAAATACTTCATTTTTTGATCCTGCTGGAGGTGGTGACCCCATCCTATACCAACATTTATTC
