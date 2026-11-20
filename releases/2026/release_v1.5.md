<div
    class="gap-10 w-full max-md:max-w-full text-sky-800"
    style="
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        margin-bottom: 0.375rem;
    "
>
    <h2 class="self-stretch my-auto text-base font-bold leading-none">Version v1.5.0</h2>
    <h3 class="self-stretch my-auto text-sm font-normal leading-none">November 2026</h3>
</div>

In the November 2026 1.5.0 release, we have added three new datasets from the Javed Khan Lab: Genomic Landscape of Rhabdomyosarcoma, Tumor Mutational Burden and the Immune Landscape of Glioma, and Immunotranscriptomic Landscape of Pediatric Extracranial Solid Tumors. We have also updated the Molecular Characterization Initiative dataset with data from additional participants and a modified clinical header description for Age at Diagnosis. In the “Pediatric solid tumor PDX dataset (UTHSA – UT Health San Antonio, 2023),” we renamed the submitter’s DATA_TYPE column, which indicated “PT” or “PDX,” to SAMPLE_CLASS because it created a second “Data Types” table on the study summary page, alongside the built-in Data Types table that cBioPortal generates. Please visit the [Dataset Updates](dataset-updates) section for more information about the latest data additions and updates.

Regarding functional updates, we fixed two bugs - one resulting in a table misalignment in the OpenPedCan dataset and one causing a 403 error on patient pages. We have also made 508 fixes to improve color contrast on the home page and have addressed key security vulnerabilities.
