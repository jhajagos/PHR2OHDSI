## Colab Notebooks for Mapping XML CDAs for Analytics

This repository brings together several Colab Notebooks for converting CDA XMLs to OHDSI
parquet files. This allows an individual to convert a personal health record to a format 
compatible for performing analysis.

The requirements for these notebooks is that you have a Google account. You have signed up 
with  https://colab.research.google.com/ and https://drive.google.com/ and familiar with
these services.

### What is a XML CDA

#### Extracting XML CDAs from Patient Portals

#### Extacting XML CDA from the Apple Health App

### Risks (Read This Before Preceeding!!!)

XML CDAs differ in quality across different EHR portals. The code here has been tested on only a subset
of CDAs available to the author. This code is developmental code to explore if XML CDAs have suitablity
data analysis. 

All analyses done with CDAs is for education purposes only and any medical decisions made should be
done with a licensed health care provider.

By uploading CDAs to Google Drive you assume risk that identifiable information could be disclosed. If privacy is of concern
these pipelines can be run on a local system using Docker. For security you should enable multi-factor authentication
for your Google Account and not share your Google Drive Folder.

### Converting to Prepared Source


### Converting to OHDSI 

