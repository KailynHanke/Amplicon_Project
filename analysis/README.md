# Analysis Folder README

This folder includes necessary analysis (and their associated rendered html) files including:

- 01_QualityTrimming.Rmd: Here I created quality plots to asses pre- and post-quality trimming. I have also created files that include the filtered and trimmed data.


- 02_AssignASVs.Rmd: In this document I assigned ASVs on both forward and reverse reads by applying the error model, and then merged forward and reverse ASVs into "contiguous ASVs". I did quality trimming of ASV lengths, removed chimeras and assigned taxonomy with the Silva Database.


- 03_PreProcessing.Rmd: I combined my data into a phyloseq object and removed any contmainating ASVs that were chloroplasts or mitochondria. I evaluated (or tried to evaluate) for controls. I also checked for reverse complements and the sequencing depth.


- 04A_Phylogenetic_Tree_Construction.Rmd: The goal of this analysis document is to make a phylogenetic tree so I can use it for phylogenetic community analyses like phylogenetic Hill Numbers and the UniFrac beta-diversity measures. 


- 04B_Phylogenetic_Tree_Inspection.Rmd: Here I merged the unrooted phylogeentic tree with my `raw_preprocessed_phyloseq` object. I then inspected and pruned my tree before mid-rooting the tree. I then combined the new, rooted tree with the phyloseq object to create a rooted tree phyloseq object.


- 05_Biodiversity.Rmd: I calculated the Hill Numbers of the samples using the iNEXT package. I then plotted and evaluated the interpolated and extrapolated rarefaction curves from iNEXT. I then analyzed the Hill numbers and then worked to answer my specific questions related to alpha diversity. Ultimately with this document I ran an analysis on the within-sample biodiversity of the samples in our project. 


- 06_Ordination.Rmd: In this document I evaluated sequencing depth and normalized the read counts between samples. I then calculated community dissimilarities and ran statistics with PERMANOVA and betadispR before visualizing the community data with ordinations (PCoA and NMDS plots).
    

- 07_Composition.Rmd: In this document I carried out a microbial compositional analysis of dairy samples across a skim milk processing pipeline. To do this I calculated th relative abundances of taxonomic groups at various levels (phylum, genus, ASVs) and then made some nice visualizations of how the microbial taxa vary across the dairy sample types.


- 08_Seasonality_Biodiversity.Rmd: The goal of this document is to run an analysis on the within-sample biodiversity of the samples in my project, similar to the analysis that I ran in 05_Biodiversity. But, this time, separating the dairy samples up not just by sample type, but by season too.


- 09_Seasonal_Ordination.Rmd: The goal of this document is to run an analysis on the between-sample (beta) diversity of the samples in my project, similar to the analysis that I ran in 06_Ordination. But, this time, separating the dairy samples up not just by sample type, but by season too.


- 10_Seasonal_Composition.Rmd: The goal of this document is to run an analysis of microbial composition of mid- and late-lactation dairy samples across a processing pipeline, similar to the analysis that I ran in 07_Composition. But, this time, separating the dairy samples up not just by sample type, but by season too.
