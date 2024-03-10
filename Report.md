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
The paper discusses the development of the effector index, utilizing GWAS summary statistics or individual-level genetic data. All data and code mentioned in the original paper are accessible online, although the data preprocessing and evaluation codes used is not provided. Positive control genes for evaluation were sourced from databases such as the Human Disease Ontology database, OMIM linkage information, and a study by Morris et al. Additionally, GWAS summary statistics were gathered from various publicly available resources and through GWAS conducted on UK Biobank traits. The paper thoroughly identifies all other data sources utilized in the study.

### Quality of experimental design	
The experimental design is clearly delineated, with each step thoroughly explained. Hyperparameters in XGBoost, such as tree depth, lambda, and gamma, were fine tuned to optimize cross-validated performance on training data. Performance evaluation was conducted using the area under both receiver operating characteristic curves (AUC-ROC) and precision-recall curves (AUC-PRC) on test datasets, ensuring comprehensive assessment of model effectiveness.

### Description of methods	
They provided a detailed flowchart of the method, which begins with fine-mapping of GWAS summary statistics, followed by annotation of single nucleotide variants (SNVs) to identify potential causal variants and their association with genes within or near the GWAS loci. Subsequently, these data are leveraged to generate gene- and locus-level features, integrating information on the presence of specific SNVs within genes, their functional implications, and locus-specific characteristics. Feature weights within the models are determined through leave-one-out analysis, facilitating the assessment of model robustness and generalizability. The performance of the models is then evaluated by predicting target genes for loci containing positive control genes, with comparisons made to known positive control genes. This evaluation aims to measure the model's accuracy in identifying true target genes while minimizing false positives and false negatives, thus providing insights into its effectiveness in prioritizing genes at GWAS loci.

### Description of sample population/data under study	
The data utilized in the study consists of GWAS data associated with 12 common traits. These traits include Type 2 diabetes, estimated bone mineral density, diastolic blood pressure, height, hypothyroidism, red blood cell count, systolic blood pressure, calcium, direct bilirubin, glucose, low-density lipoprotein, and triglycerides. This diverse range of phenotypes or conditions provides a comprehensive dataset for the analysis and development of the effector index discussed in the study.

### Tool accessibility 
The tools required for the study are publicly available, although the algorithm is implemented in a mixture of Shell and R. Despite their availability, the absence of a guideline or readme file may pose challenges in utilizing these tools effectively. This lack of documentation could potentially hinder users' ability to understand and apply the algorithm, thus reducing its accessibility and usability. 

### Replicability 
The algorithm utilized in the study can be replicated for use with GWAS data associated with different traits. However, replicating the data preprocessing steps may present challenges as the code for this process is not provided. Lack of access to the preprocessing code could hinder the replicability of the study, as it may be difficult for other researchers to precisely reproduce the initial data preparation steps. Providing the preprocessing code or detailed instructions would enhance the replicability of the study and facilitate its adoption by other researchers interested in utilizing similar GWAS datasets.

### Molecular Biology
## Paper 1 (LH): Single-molecule tracking reveals the functional allocation, in vivo interactions, and spatial organization of universal transcription factor NusG (2024)

### Data availability and accesibility
This paper is published under open access. A key resource table is provided which lists all reagents, bacteria strains, data and software etc., their source and identifier (if applicable). Fluorescence imaging dataset is published and openly available on Mendeley. Links are provided to the sources of the code and softwares used, however one of the softwares is reported to be no longer supported. Contact information is provided for the lead author along with a statement acknowledging information will be provided upon request if needed to reanalyze the data. A statement is provided acknoledging that all strains generated in the study will be provided upon request. All this information was provided in a section called STAR Methods. STAR stands for Structured, Transparent, Accessible Reporting. This is a methods format introduced in 2016 that has been adopted by all Cell Press journals (https://www.cell.com/star-authors-guide).

### Quality of experimental design
- Sequencing was performed on the constructs as validation
- Bootstrapping analysis is performed to calculate fitting errors for the D* distributions
- In the methods there is a statement claiming experimental repeats were performed for each condition to define the reproducibility of the results however I don't see anywhere in the paper where this reproducibility is quantified.
- Many conditions were tested to solidify their conlcusions regarding the different NusG populations and their corresponding functions/interactions. For each of these conditions a similar number of NusG molecules were observed (order of 10 000), maintaining similar statistical power for each measurement. For example, when characterizing the fast population, three different conditions were measured improving the robustness of their conclusions (as oppose to making a conclusion from one condition).

### Description of methods
- There is a clear, specific description of the methods used to create each new bacterial strain. For construction procedures that are well known, references are provided to early papers that give in depth details of the procedure. A supplemental table is also provided outlining the names of each strain, their use for the paper and their genotype.
- The methods described for immunoblotting contained specific details regarding temperatures, times, volumes, and reagents. I have not performed immunoblotting but I feel that the methods described here are specific enough that I would be confident with replicating the procedure.
- Cell preparation methods go into very specific details, explicitly stating all variables invovled in this process
- For single molecule imaging, the various parts of the custom built microscope (lasers, camera, objectives, modulators, etc.) were explicitly stated along with their respective provider and identifying code. Additionally the acquisition details were provided.
- SIM imaging acquisition details were described in depth. Additionally, references are provided directing to papers with further details on the 3D imaging procedure.
- For single molecule tracking analysis a reference is provided to a previous paper where the same method was used. A brief description is also provided, while the methods in the previous paper are in great depth.

### Description of sample population/data under study	
This study is examining the dynamics of NusG (a molecule) in E. coli to make inferences about the different NusG populations and their abundance. One could thus claim that the sample population is the NusG molecules. For each distribution that was reported the number of NusG molecules contributing to the distribution was reported in the figure caption which averaged around 40 000. These molecules were sampled from many E. coli cells (order of hundreds) in multiple fields of view (not specified numerically). For this type of study, I would claim that the sample population is representative (not just collected from one experiment/ one field of view / one experiment). One improvement would be including the number of fields of view and experimental repeats with the statement made in the Quantification and Statistical Analysis statement. 

### Tool accessibility
- The microscope used for single-molecule tracking PALM is custom built, thus it is not easily accessible unless you are located at their institution (Oxford). A detailed description regarding the microscopes specs was provided which allows people to identify a commercial microscope that is comparable.
- The microscope used for SIM imaging is commercial - more accessible than custom built
- Single molecule localizations performed with custom software
- As previously stated, links are provided for open access code and software that were used for analysis.
