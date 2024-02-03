# Strand-Depedent-TF-Binding
An R notebook to graph TF (or histone modification) average signal intensity over a list of target TAIR10 genes

This script will take a target genes list and a bedgraph from a protein or histone modification of interest, split the genes of interest based on the Wattson or Crick strand, and graph the average signal intensity of the protein or modification with respect to the transcriptional start site. 

Lines 12 through 17 are designed to be edited with paths to your gene list of interest, a path to the Arabidopsis GTF, a path to your bedgraph file, your desired y-axis label, your start position (listed as a negative upstream number), and your end position (listed as a positive downstream number)

In the Multi GeneLists and Bedgraph file, the code block starting at line 13 requires user editing including paths to bedgraphs, paths to gene lists, and information about datasets. 

Using the function option, users only need to give the function two input files and start and end numbers from the transcription start site. 
This function is inspired by DESeq2's file input. Here, two 2 by x tables are made, one containing gene lists of interest and a description of the file, the other containing bedgraphs and a description of the file. 
The meanPlot function requires 4 inputs, the gene list table, the bedgraph table, a point upstream of the start codon (start), and a point downstream of the start codon (end). Additionally, users can specify an input file to normalize IP data against over the gene list. 
