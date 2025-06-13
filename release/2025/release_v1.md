## Version v1.0.0
### May 1, 2025
The 2.6.0 quarterly release (April 2025) of the CCDI Hub features a modified data model, new data, and new features for browsing and selecting cohorts. Three new data sets have been added from TARGET, Acute Lymphoblastic Leukemia (ALL) Pilot Phase 1 (PHS000463), Acute Lymphoblastic Leukemia (ALL) Expansion Phase 2 (PHS000464), and Acute Myeloid Leukemia (AML) (PHS000465), and a field has been added to capture study status. Participants who were no longer eligible were removed from Molecular Characterization Initiative (PHS002790) and TARGET: Kidney, Wilms Tumor (WT)(PHS000471) studies. Explore Dashboard facet updates include a new facet for the study status property, propagation of facet text search to Sample Anatomic Site, and an increase of the participant set upload limit to allow for upload of 5,000 Participant IDs. Numerous updates have been made to the Explore Dashboard Participants table, including new fields, customizable columns, a feature for creating cohorts, and mapping of associated information from the CCDI Participant Index (CPI). The Molecular Characterization Initiative (MCI) page has been updated with February 2025 enrollment summaries and a new link to a COG transformation script in a GitHub repository. General updates include new links from the Home page and Resources menu, a dedicated Release Notes page, and more.

Additional details are listed below:

#### CCDI Hub Data Updates

##### Data Model Updates
- Added more properties to Treatment node  
- Added slim_url property for IDC imaging data
- Added study status
- Renamed &quot;COG Clinical Report&quot; to &quot;COG Clinical Data&quot;
- Updated synonym properties to include CPI mapping data

##### New Data Sets
- CCDI Pediatric In Vivo Testing Program - Neuroblastoma (PHS003163)
- TARGET: Acute Lymphoblastic Leukemia (ALL) Pilot Phase 1 (PHS000463)
- TARGET: Acute Lymphoblastic Leukemia (ALL) Expansion Phase 2 (PHS000464)
- TARGET: Acute Myeloid Leukemia (AML) (PHS000465)

##### Updated Data Sets
- CCDI Pediatric In Vivo Testing Program - Leukemia (PHS003164)
- Comprehensive Genomic Sequencing of Pediatric Cancer Cases (CMRI/KUCC) (PHS002529)
- Enhancement of Data Sharing in Pediatric, Adolescent and Young Adult Cancers (PHS002431)
- Genomic Sequencing of Pediatric Rhabdomyosarcoma (PHS000720)
- Identification and Targeting of Treatment Resistant Progenitor Populations in T-cell Acute Lymphoblastic (PHS003432)
- Integrating Longitudinal Clinical, Sociodemographic and Genomic Data into the NCCR (PHS002677)
- Molecular Characterization across Pediatric Brain Tumors and Other Solid and Hematologic Malignancies for Research, Diagnostic, and Precision Medicine (PHS002517)
- Molecular Characterization Initiative (PHS002790)
- OncoKids - NGS Panel for Pediatric Malignancies (PHS002518)
- TARGET: Kidney, Clear Cell Sarcoma of the Kidney (CCSK) (PHS000466)
- TARGET: Kidney, Rhabdoid Tumor (RT)(PHS000470)
- TARGET: Neuroblastoma (NBL) (PHS000467)
- TARGET: Osteosarcoma (OS) (PHS000468)
- UCSF Database for the Advancement of JMML - Integration of Metadata with Omic Data (PHS002504)

##### Removed Data Sets
- Feasibility and Clinical Utility of Whole Genome Profiling in Pediatric and Young Adult Cancers (PHS002620)
- Clonal evolution during metastatic spread in high-risk neuroblastoma (PHS003111)

#### CCDI Hub Site Updates
##### General Site
- Added tab under News page for release note notifications
- Added ecDNA resource block on Home page and menu link from Resources menu
- Added dedicated page to display full release notes
- Made persistent link to user guide from About menu
- Updated user guide

##### Molecular Characterization Initiative (MCI) page
- Added link to COG transformation script GitHub repository
- Increased text thickness to improve readability
- Fixed bug resulting in unintended outlines when interacting with donut chart
- Removed alt text unintentionally appearing in main page text under image
- Updated enrollment counts as of February 2025

#### CCDI Hub Explore Dashboard
##### Facet update
- Added facet for study status
- Added text search option to sample anatomic site facet
- Increased participant set upload limit to 5,000

##### Tables
- Added cohort selector feature to Participants tab
- Added column to display study status
- Added commas to all numbers larger than 1,000 in table headers and pagination
- Added fields from Treatment, Treatment Response, and Survival nodes to Participants tab
- Added indicator, hover dialog, and popup table summary for participants with additional information mapped in the Cancer Participant Index (CPI)
- Changed column label &quot;Sex&quot; to &quot;Sex at Birth&quot; to match model
- Exposed properties under generic_file node
- Made visible columns customizable by checkbox selection
- Removed separate Diagnosis tab and moved relevant fields to Participants and Samples tabs

##### Cart
- Added commas to all numbers larger than 1,000 in table headers and pagination and in cart icon
