## CCSS Therapy-Related Mutation Signatures in Subsequent Neoplasms
The Childhood Cancer Survivor Study (CCSS) is a large, multi-institutional research effort that tracks long-term health outcomes in people who were diagnosed with cancer as children or adolescents and survived at least five years. The clinical, expression, and alteration data ingested into the CCDI cBioPortal were derived from the study Brady et al. Cancer Discov. 2026 supplementary tables unless otherwise specified. The underlying CCSS sequencing data can be explored through the [CCDI Hub Explore](https://ccdi.cancer.gov/explore?dbgap_accession=phs001327) using study accession phs001327, with access to controlled-access data requiring authorization through [dbGaP](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=phs001327). Note: Sample IDs in the CCDI cBioPortal study were re-formatted from publication supplementary tables to match the sample IDs used in CCDI indexed study (phs001327) for interoperability between the data repositories.


### Clinical Data
Clinical data (diagnosis, staging, treatment, receptor status and histology) were sourced from Supplementary Table 1 of the Brady et al. Cancer Discov. 2026 study. The most recent available status and timepoints to determine overall survival time and status were extracted from the data submitted to CCDI.


### Mutation Data
Driver mutations, SNVs, and indel variants in tumor mutational burden analyses were obtained from Supplementary Tables 1, 6 and 11, respectively. The variants were formatted and then annotated with the [Genome Nexus Annotation Pipeline](https://github.com/genome-nexus/genome-nexus-annotation-pipeline) to additionally provide annotations required for ingestion of mutation data. Mutations were then labeled with their source type, i.e. “Kind Type” field, as either “Driver” or “SNV/Indel TMB” (Tumor Mutational Burden), enabling users to filter variants accordingly. Tumor variant allele fraction (VAF) data were also included for TMB SNVs and indels, as reported in Supplementary Tables 6 and 11.


### Structural Variant Data
Driver fusion and structural variants were extracted from Supplementary Tables 21 and 23. For fusions or rearrangements with one breakpoint in an intergenic region, ‘Intergenic’ was used as the HUGO Symbol placeholder; these will appear with a blank ‘Gene’ field in the gene-level ‘Structural Variants’ table.


### Copy Number Data
For focal driver copy number alterations listed in Supplementary Table 1, GISTIC-like values were mapped to the values provided for discrete copy-number alterations:

| S. Table 1 Copy Alteration | Discrete Alteration in cBioPortal |
| --- | --- |
| focal_amp | Amplification |
| focal_gain_low-level | Gain |
| focal_del | Shallow Deletion |
| focal_HomDel | Homozygous Deletion |

Chromosome 22 loss status from Supplementary Table 1 was included as a clinical variable.
