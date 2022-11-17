# Strand-Depedent-TF-Binding
A simple R notebook to graph TF (or histone modification) signal intensity over a list of target TAIR10 genes

This script will take a target genes list and a bedgraph from a protien or histone modificication of interest, split the genes of interest based on the Wattson or Crick strand and graph the average signal intensity of the protein or modification with respect to the transcriptional start site. 

Lines 12 though 17 are designed to be edited with paths to your gene list of interest, a path to the Arabidopsis GTF, a path to your bedgraph file, your desired y-axis label, your start position (listed as a negative upstream number), and your end position (listed as a positive downstream number)
