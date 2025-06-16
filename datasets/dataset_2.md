## Molecular Characterization Initiative
### Mutation Data
#### April 8, 2025

The MCI mutation data was sourced from controlled access VCFs from dbGaP: dbGaP Study (phs002790.v1.p1). These VCFs were generated from CLIA-compliant enhanced paired tumor–normal exome sequencing conducted by the Steve and Cindy Rasmussen Institute for Genomic Medicine (IGM) at Nationwide Children's Hospital in Columbus, OH. These were somatic VCFs where germline variants had been filtered out.

The variants in each VCF file were ran thru the vcf2maf tool, which employs the following steps:

1. The VCF file format is first converted to MAF format, which calculates end position of the variant and strand information as well as transforms data from columns in the VCF file to match the standard MAF format.

2. The variants in MAF format are then annotated by Ensembl's VEP (Variant Effect Predictor) tool (which is wrapped in the vcf2maf tool) which selects a single "effect" per variant and provides variant level annotations from a variety of other databases and sources such as rsID from dbSNP, amino acid change, variant classification (e.g. Silent, Missense, Nonsense, In Frame Insertion/Deletion etc.), and others.

The individual MAF files were then concatenated into a single MAF for loading into cBioPortal. The concatenated MAF was then filtered to retain only mutations that were marked as passing all quality filters in the VCF.

Note: This data filtering approach may not match other CCDI/GDC data sources.
