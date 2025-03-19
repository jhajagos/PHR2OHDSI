## Colab Notebooks for Mapping XML CDAs for Analytics

This repository brings together several Colab Notebooks for converting CDA XMLs to OHDSI
Parquet files. CDAs are structured documents which can be downloaded from 
from a health system's patient portal.  The Colab Notebooks allows an individual to convert 
disparate records to an industry standard OHDSI Common Data Model (CDM) for analysis.

The primary requirements for these notebooks is that you have a Google account. You have signed up 
with  https://colab.research.google.com/ and https://drive.google.com/ . You should be familiar with 
uploading files to Google Drive, basic familarity with Python, and running notebooks in Colab.

### What is an XML CDA

CDA (Consolidate Document Architecture) is a document used to encode digital health information
from Electronic Health Record (EHR).

#### Extracting XML CDAs from Patient Portals

#### Extacting XML CDA from the Apple Health App

### Risks (Read This Before Preceeding!!!)

XML CDAs downloaded from EHR portals vary in quality. The code here has been tested on only a subset
of CDAs available to the author. This code is written to explore the potential of utilizing 
XML CDAs for data analysis. 

All analyses done with CDAs is for education purposes only and any medical decisions made should be
done in partnership with a licensed health care provider.

By uploading CDAs to Google Drive you assume risk that identifiable information could be disclosed. 
If privacy is of concern these pipelines can be run on a local system using Docker. 

For security you should enable multi-factor authentication for your Google Account and not share your 
Google Drive Folder with other users. 

### Converting to Prepared Source

Create a new folder in your Google Drive called `phr_ohdsi`. Create a subdirectory within it called `fml_docuemnts`.
Upload your CDAs XML dcoument to this folder from your local computer. 

Set the following variable in the notebook `Map_CDAs_to_OHDSI_CDM_in_a_Colab_Notebook.ipynb`

```python
CDA_FILE_PATH = "/content/drive/MyDrive/phr_ohdsi/source/jgh_documents/"
```
See the next section for setting `OHDSI_VOCABULARY_PATH`.

### Converting to OHDSI 

To fully convert your CDAs to OHDSI CDM you will need to download and stage your OHDSI vocabulary files. Create a directory in
in your Google Drive called `OHDSI` and a subdirectory called `vocabulary` and create a further sub-directory based on the date `20250317`. 
In tne notebook
`Process_OHDSI_Vocabularies_For_Mapping.ipynb` update the variable to point to this directory

```python
OHSDI_VOCABULARY_PATH = "/content/drive/MyDrive/OHDSI/vocabulary/20250317/"
```
