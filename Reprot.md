---
output:
  pdf_document: default
  html_document: default
---
# Reproducibility of Papers on Different Fields

## Notes

## Microbiology

## Paper 1: Cartography of opportunistic pathogens and antibiotic resistance genes in a tertiary hospital environment (2020)

### Data availability and accessibility
The paper was published under open-access. The original fastq sequencing data (as well as SRA and BAM files) have been made available through an accessible online database (Project PRJEB31632) in the European Nucleotide Archive with a link to the database page embedded within the published paper. A significant amount of supplementary data (e.g. metadata, taxonomic and resistome profiles, patient isolates) that was not published in the main article are also available; this supplementary data was also analyzed and 13 supplementary figures and 3 notes are provided to readers as a part of the publication (via free download from the Nature Medicine website). 

### Quality of experimental design	
This particular research is an observational study with spatio-temporal specificity. Therefore, certain criteria such as blinding and randomization of samples were not appropriate for this particular work. Technical replicates were not performed for environmental sampling nor culture enrichment of swabbed samples. Controls, spike-ins, and validation experiments were performed for kit (i.e. reagents and DNA extraction kits, etc.) contamination effect on environmental samples, particularly low biomass samples. Negative control swabs were performed to monitor swab contamination. Data exclusions were clearly acknowledged (e.g. samples with low DNA yield below sequencing threshold) and the number of total exclusions (3 out of 358 DNA libraries) were provided by the authors. For significant results discussed in the paper, the type of statistical analysis, resulting P-values, and accompanying assumptions were provided within the results. The paper is also accompanied by a "Reporting Summary" which Nature Research implemented to improve reproducibility and transparency in their published works. This Reporting Summary very clearly outlines the life sciences study design and makes it easy for the reader to understand the design limitations and reasons why a design method was selected for the undertaken research. No conflicts of interest were noted.

### Description of methods	
The methods are detailed and quite lengthy; therefore, seemingly to maintain clarity, the methods section was published at the end of the publication following the references section. Additionally, the references cited within the methods section were listed inside the methods section in a type of sub-references section. This also improved clarity as it helps with  cross-referencing papers used in the method development. The paper concludes that culture enrichment of low-abundance resistant pathogens combined with long read sequencing is powerful and suitable for recovering genomes without isolation. Although a very exciting work, the paper does not describe if "laboratory artifacts" are introduced to bacteria-of-interest during the enrichment step: the facilitation of bacterial conjugation to exchange resistance-encoding genes could be problematic to the concluding results if true. 

### Description of sample population/data under study	
Due to the observational nature of this study (i.e. antimicrobial resistance surveillance study), the sampling population is limited to various locations within one tertiary hospital in Singapore. Bias of sample selection (whether environmental or clinical) could arise due to this inherent limitation in sampling large areas under study. This paper also uses previous data collected using different methods performed over a decade ago. Interestingly, using these two data sets, they found five nearly identical strains of Staphylococcus aureus persisting in the same hospital environment for over 8 years at the time of the research work. However, it is unclear if these strains were stable for the entire duration or were reintroduced at some point.

### Tool accessibility 
All software used and their respective versions used are explained in detail. The statistical analyses were "performed in R" but no packages were described (if used). The equipment and reagents used were also described in detail in the methods section and their respective commercial sources were also listed. 

## Paper 2: Linking the resistome and plasmidome to the microbiome (2019)

### Data availability and accessibility
The paper was originally published in 2019, and its publishing journal became fully open access on January 1st 2024. The original fastq sequencing data are available through an accessible online database (Project PRJNA50646) in the Sequence Read Archive data repository. Supplementary data and code for analyses that was not published in the main article are also available through OSF Home, a free open platform for data sharing, and which was provided by the private research partner. 

### Quality of experimental design	
It is unclear how many replicates of the sequence libraries were made: the study describes taking a single wastewater sample at one time point and splitting it into sub-samples but does not elaborate. A single positive control of known bacteria with a sequenced plasmid was spiked to a subset of the environmental wastewater sample to maintain a known 10% concentration. The study concludes that spurious links found in the bioinformatics analysis were probably related to the high abundance of this spiked organism, resulting in some clusters relating to other organisms that were not expected to have had any relation to the plasmid. No follow-up or additional evidence as to why this was observed or if this was a statistically significant conclusion was provided. No discussion of the type of statistical analyses on the environmental sampling data were performed; statistical assumptions or significance statistics were not provided. Additionally, there are some methods that could be written in more detail, for example, it is unknown if cell pellets isolated from wastewater were frozen at -20 degrees Celsius in a storage buffer (e.g. glycerol solution), water, or just as a dry pellet: in this case, storage of unprotected cell pellets can be significantly damaged by freeze-thaw during sample processing and could impact inference of the data. Data exclusions were recognized and acknowledged, and reasons why provided; the authors discarded all contigs less than 1000 base pairs in size or which contained fewer than two restriction enzyme sites contig-cluster linkages represented by only one or two reads. Conflicts of interest were acknowledged in the paper: three of the authors are employees and shareholders of Phase Genomics, and two of these three are also executives of the company. 

### Description of methods	
The methods section fails to accurately describe the proximity ligation step of the protocol; the authors did not describe the DNA binding step (e.g. using formaldehyde) prior to cell lysis within the article body; the authors did refer to the use of the commercial ProxiMeta Hi-C Preparation Kit by Phase Genomics to create the Hi-C library but further inspection of the Hi-C Preparation Kit protocol (which was not linked to in the article) has the reagents listed with generic names (e.g. Crosslinking buffer) rather than chemical names and their respective components. The authors did include Figure 1a which depicts this covalent bonding step (via formaldehyde), although prior to the Hi-C library construction, though this is not clearly described in the methods section. Inadvertently, this could be very confusing for readers not familiar with the covalent binding step of cell nucleic acids for proximity ligation. Additionally, the flow cytometry protocol for environmental cell counts was not described.

### Description of sample population/data under study	
The title of the paper, "Linking the resistome and plasmidome to the microbiome"" is too generic and could be misconstrued as misleading. For this paper, the title should allude to the fact that only one wastewater sample was taken at a single time point in October 2017, and then split into fractions (in which only one was spiked) and analyzed. The extrapolation of this small sample set to any other environmental, clinical, human, or animal microbiome environment is far-reaching at best. There is no provided metadeta of the wastewater sample (e.g. pH, total and volatile solids content, chemical oxygen demand, fecal coliform concentrations, ammonia/ammonium, organic acids, etc.) which greatly impact not only microbial cells and their growth but also downstream processing. This paper is at its heart a methodological validation experiment, and therefore the poor characterization of samples is exasperating. 

### Tool accessibility 
Software used was provided, though exact versions used were not always described. Analyses of the Hi-C libraries were performed using a proprietary pipeline developed by the private research partner and was acknowledged in the paper. Not all of the equipment and reagents used were described in enough detail in the methods section, for example, the make and model of the flow cytometer used for cell counts was not described nor the "R2A agar" media for colony forming unit (CFU) counts was not provided with a recipe list nor the commercial vendor (if applicable). 

## Genetics
## Paper 6: Human genetics evidence supports two-thirds of the 2021 FDA-approved drugs (2022)
### Data availability and accessibility
The paper was originally published in Nature Reviews Drug Discovery under the biobusiness briefs section. The codes are accessible, with the link provided in the article. However, the platform used to store their data is unavailable.

### Quality of experimental design	
The study aims to find genetic support for FDA-approved drugs. For the experimental design, it utilized 15 different databases to identify evidence.

### Description of methods	
The methods are explained in the supplementary documents. Initially, Drug IDs were converted to Gene IDs, followed by leveraging 15 different genetic resources as integrated by the Open Targets Platform. Related traits to the drug indication were manually included, with the availability of genetic evidence for the drug target.

### Description of sample population/data under study	
They used 15 different genetic resources, which is very comprehensive and covers a wide range.

### Tool accessibility 
The code and data are available online, but the software used to store their data, known as "spark," is not accessible without Google Cloud storage, which requires payment.

## Paper 7: An effector index to predict target genes at GWAS loci (2021)
### Data availability and accessibility

### Quality of experimental design	

### Description of methods	

### Description of sample population/data under study	

### Tool accessibility 

### Replicability 
