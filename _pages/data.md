---
permalink: /data/
title: "Data"
excerpt: "Read about - and download - the data here"
author_profile: true
redirect_from: 
  - "/data"
  - "/data.html"
---

## Spine of all third sector organisations

The initial data product of this project is a spine of all UK third sector organisations, their names, addresses and dates of registration (and dissolution where relevant).
Additionally, where organisations are found in more than one register, we provide a file listing these linkages. Data relating to alternative names and addresses is also
collated for completeness.


The organisational spine consists of three csv files: 

+ public\_spine.spine.csv contains a row for each organisation considered to make up the UK's thrid sector, with name, address and date details. 
+ public\_spine.supplementary.csv contains any name, address and date information associated with an organsiation which is additional to what is in the spine, 
such as 'Also Known As' names, previous addresses. 
+ public\_spine.matches.csv lists the organisations which are linked or matched according to our searches, along with the type of match. 

## Download spine files 
These three files can be downloaded using these links:  
+ <a href="https://github.com/uk-third-sector-database/tso-database-builder/raw/main/tso-spine-files.16-7-24.zip?download=" download>Download zipped csv files : Release #2 (16-7-24).</a>
+ <a href="https://github.com/uk-third-sector-database/tso-database-builder/raw/main/tso-spine-files.4-7-24.zip?download=" download>Download zipped csv files : Release #1 (4-7-24).</a>

## Data dictionaries

### Main organisational spine
The file containing the list of unique organisations comprising the third sector, public_spine.spine.csv, contains the following fields:

| Fieldname         | Notes                                                                                       |
|-------------------|--------------------------------------------------------------------------------------------|
| uid               | UID created for each source, e.g. GB-CHC-1234                                              |
| organisationname  | Name as primary in source                                                                  |
| normalisedname    | Name normalised to capitalise, remove extra spaces and punctuation - to aid matching        |
| fulladdress       | Full address as found in source with highest precendence across any matched organisations   |
| city              | City matching full address as defined above                                                 |
| postcode          | Postcode matching full address as defined above                                             |
| registerdate      | Earliest registration date found in records for this organisation across all sources        |
| removeddate       | Latest dissolution date found in records for this organisation across all sources           |


### Supplementary information
File of supplementary data for organisations, public_spine.supplementary.csv, contains the following fields:

| Fieldname         | Notes                                                    |
|-------------------|----------------------------------------------------------|
| uid               | UID created for each source using source and id from original source |
| organisationname  | Alternative name                                        |
| normalisedname    | (Alt name normalised)                                   |
| fulladdress       | Alternative address                                     |
| city              | Alternative address                                     |
| postcode          | Alternative address                                     |
| registerdate      | Alternative registration date                           |
| removeddate       | Alternative removed / dissolved date                    |


### Matches
Matches between organisations are listed in file public_spine.matches.csv, using the following fields:

| Fieldname          | Notes                                                                                                     |
|--------------------|-----------------------------------------------------------------------------------------------------------|
| uid                | UID created for each source, matches table  - if match is unambiguous; blank otherwise |
| orgA_id_in_source  | ID in original source, for matched organisation A                                                           |
| orgA_source        | Original source of organisation A                                                                          |
| orgA_uid           | UID created for organisation A                                                                             |
| orgB_id_in_source  | ID in original source, for matched organisation B                                                           |
| orgB_source        | Original source of organisation B                                                                          |
| orgB_uid           | UID created for organisation B                                                                             |
| match_type         | Type of match (e.g. by name, by companyid)                                                                 |


