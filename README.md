# Data-Wrangling
An example of working with relational databases in R

We have an excel workbook containing related tables that we wish to merge into a cohesive report. 
Tables contain information for patient clinical data, serum protein assays, tissue sample metadata and the associated RNA sequence results.



Data Specification:
Study_ID: The GEO study number, from the file name
Patient_ID: The unique patient identifier, from the Patient Clinical Data worksheet
Unique_Patient_ID: Concatenation of the STUDY_ID and the Patient_ID with underscore
Sex: The sex of the patient
Age: Age (in years) at time of diagnosis
Sample_ID: Unique sample identifier
Sample_General_Pathology: For the tumor samples only, the pathology of the sample interpreted from the Tissue Sample Metadata table, Sample Type 
Material_type: The processed sample used to perform the assay
Gene_Symbol: Gene symbol for the transcript or protein assayed
Result: The value of the assay, provided in the data tables, corrected for any non-standard units. Missing data or non-numeric values are reported as null.
Result_Units: The units used to express the results
Status: If a valid result exists, this value is null. For any non-valid or missing value, report "NOT DONE"


