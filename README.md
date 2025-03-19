## Colab Notebooks for Mapping XML CDAs for Analytics

This repository brings together several Colab Notebooks for converting CDA XMLs to OHDSI
Parquet files. CDAs are structured documents which can be downloaded from 
from a health system's patient portal.  The Colab Notebooks allows an individual to convert 
disparate records to an industry standard OHDSI Common Data Model (CDM) for analysis.

The primary requirements for these notebooks is that you have a Google account. You have signed up 
with  https://colab.research.google.com/ and https://drive.google.com/ . You should be familiar with 
uploading files to Google Drive, basic familarity with Python, and running notebooks in Colab.

### What is an XML CDA

CDA (Consolidate Document Architecture) is a docuemnt used to encode digital health inforamtion
from Electronic Health Record (EHR).

#### Extracting XML CDAs from Patient Portals

#### Extacting XML CDA from the Apple Health App

### Risks (Read This Before Preceeding!!!)

XML CDAs downloaded from EHR portals vary in quality. The code here has been tested on only a subset
of CDAs available to the author. This code is developmental code to explore if XML CDAs.

All analyses done with CDAs is for education purposes only and any medical decisions made should be
done with a licensed health care provider.

By uploading CDAs to Google Drive you assume risk that identifiable information could be disclosed. If privacy is of concern
these pipelines can be run on a local system using Docker. For security you should enable multi-factor authentication
for your Google Account and not share your Google Drive Folder.

### Converting to Prepared Source

Upload your CDA xml docu ents

### Converting to OHDSI 

