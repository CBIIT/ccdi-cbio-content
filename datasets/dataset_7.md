## Genomic Landscape of Rhabdomyosarcoma
The Genomic Landscape of Rhabdomyosarcoma dataset represents an integrated analysis of pediatric rhabdomyosarcoma (RMS) samples from Children’s Oncology Group (COG) and United Kingdom cohorts, as published in Shern et al. J Clin Oncol 2021 ([PMID 34166060](https://pubmed.ncbi.nlm.nih.gov/34166060/)). The dataset contains somatic mutations, copy number, RNA expression, and per-sample fusions for 780 samples across 641 patients. All samples are rhabdomyosarcoma; subtypes represented include Embryonal, Alveolar, Spindle Cell, Mixed Alveolar and Embryonal, Pleomorphic, and RMS NOS.


### Clinical Data
Clinical data were sourced from the COG UK RMS consortium and include Cancer Type (Rhabdomyosarcoma), Cancer Type Detailed (six RMS subtypes), Sex, Race, Ethnicity, Age at Enrollment, Overall Survival (OS) and Event Free Survival (EFS) with event type (Relapse, Progression, Death, or Second Malignant Neoplasm), Risk Group, Stage, Metastatic status at Diagnosis, Cohort (COG or UK), Anatomic Group, FOXO1 Fusion Status, and RAS Pathway alteration status.


### Mutation Data
Somatic mutations were called on a custom 39-gene targeted panel, and all somatic tiers were loaded with their tier annotation. Additional variants predicted as highly likely driver variants (i.e. Tier 1) from GATK HaplotypeCaller run on RNA-Seq reads were also provided and are labeled as RNA-Seq in the mutation data.


### Copy Number Data
CNVkit was used to generate per sample segment level copy number calls (hg19). Segment log2 values were mapped to gene coordinates via overlap weighted mean against UCSC hg19 refGene to produce a gene level continuous CNV matrix. Discrete GISTIC-like calls were derived from the continuous values using standardized thresholds:
* Amplification (+2): log2 > 2.0 (CN > ~8)
* Gain (+1): log2 > 0.3
* Neutral (0): -0.3 to 0.3
* Shallow deletion (-1): -1.0 to -0.3
* Deep deletion (-2): log2 < -1.0


### Structural Variant Data
Fusion calls were generated using Arriba on RNA-Seq data, mapped to GRCh37/hg19 coordinates, and loaded into cBioPortal in standard structural variant format.
