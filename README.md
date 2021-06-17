# High-quality Inter-species cross-talk identfication from dual RNA-seq transcriptomic data using XTalkiiS tool.

## Introduction
XTalkiiS, a tool for finding data-driven cross-talks between intra-/inter-species pathways depends on a gene dependency network as a input. For intra-species pathway network, such gene-dependecy network can be easily built using guilt-by-association modelling among all participating genes using some state-of-the-arts techniques, e.g. [WCGNA](https://github.com/cran/WGCNA) (correlation-based), BNMCMC (causal relationship), etc. However, for inter-species conditions, it is very difficult to model such networks as to model high quality association between two species (e.g. Host-pathogen), we need matched omics data. Fortunately, dualRNA-seq studies are one of such techniques which generates total RNA-seq transcriptomics of host and pathogens simultaneously. Hence, modelling a robust gene-dependency networks combining host-pathogen dual RNA-seq data with their respective protein-protein interactome using both correlation and causation-based techniques can be levaraged with [XTalkiiS](https://github.com/Akmazad/XTalkiiS/blob/master/README.md) algorithm  to find out inter-species pathway cross-talks between host and pathogens. These findings can later be used to quantify network-medicine principles, e.g. network-seperation of drug targets modules, drug-disease proximity analysis using [drugly](https://github.com/Akmazad/drugly) package [currently being built by us]. These results may enable us to find effective therapeutic strategies against varoius inter-species cross-talk related disease mechanisms.

## Tools [in progress]
- [BNMCMC](https://github.com/Akmazad/BNMCMC-Server)
- [WGCNA](https://github.com/cran/WGCNA)
- [drugly](https://github.com/Akmazad/drugly)
- [XTalkiiS](https://github.com/Akmazad/XTalkiiS/blob/master/README.md)

## Features
- Modeling inter-species gene-gene interaction network from dualRNA-seq data
- Integration of dual RNA-seq transcriptomics, interactomics, functational annotation data (e.g. KEGG, GO, etc.)
- Extraction of high-quality inter-species cross-talks using XTalkiiS algorithm
- Annotation of those yielded cross-talks with drug targets and their multi-modal similarity information
- Generating network-based analytics of those cross-talks types markers
- Advanced visualiztion of those results using drugly package, or [COVID-CDR](https://unsw-data-analytics.shinyapps.io/COVID_CombTherap/)  type platforms
