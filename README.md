# Descriptive analysis of immigration enforcement and detention data for the Pacific Northwest

This repository collects various sources of data from U.S. Immigrations and Customs Enforcement (ICE), Customs and Border Protection (CBP), and the Department of Justice regarding immigration enforcement, detention, and court outcomes; focusing on Washington and Oregon states.

This repository generates figures and an [interactive data appendix](https://uwchr.github.io/describe-sea/border-everywhere.html) for the report "[The Border is Everywhere: Immigration Enforcement in the Contemporary Pacific Northwest](https://jsis.washington.edu/humanrights/2024/09/05/the-border-is-everywhere-immigration-enforcement-in-the-contemporary-pacific-northwest/)" by the University of Washington Center for Human Rights, published September 5, 2024.

## Data

The datasets analyzed in this repository as of September 4, 2024 are available at the following link: https://drive.google.com/drive/folders/1N4uRkWTSTZx7zkSRc0fqyij6FouQN7SH?usp=drive_link

To generate documentation produced by code in this repository, unzip the files at the link above in the `import/input/` directory in this repository; these files are targetted by symlinks in `write/input/` which are required to Knit data appendix via `write/note/describe-sea.Rmd`.

### Data sources

This repository presents UWCHR analysis of data from multiple sources:

- ICE data on nationwide ICE enforcement events (encounters, arrests, and removals) for FY 2012-January 2023, obtained by the UW Center for Human Rights through Freedom of Information Act litigation against the Department of Homeland Security (DHS). This data is processed in the following repository: https://github.com/UWCHR/ice-enforce
- ICE detention records for FY 2012-January 2024, obtained by the UW Center for Human Rights through Freedom of Information Act litigation against the Department of Homeland Security (DHS). This data is processed in the following repository: https://github.com/UWCHR/ice-detain
- Analysis of a collection of DHS I-213 “Record of Deportable/Inadmissible Alien” forms, obtained by UWCHR through Freedom of Information Act litigation against DHS, which provide detailed narratives of apprehensions in the Seattle Area of Responsibility covering the period from January 1, 2019 to November 30, 2021. This data is analzed in the following respository: https://github.com/UWCHR/i-213-analysis
- Publicly available datasets published by Customs and Border Protection (CBP), including two sources of nationwide aggregate data on [US Border Patrol monthly encounters from FY 2000 to FY 2020](https://www.cbp.gov/document/stats/us-border-patrol-monthly-encounters-fy-2000-fy-2020) and [CBP nationwide encounters from FY 2020 to FY 2023](https://www.cbp.gov/newsroom/stats/nationwide-encounters). This data is processed in the following repositry: https://github.com/UWCHR/cbp
- Immigration court data from the Department of Justice’s Executive Office for Immigration Review (EOIR) and ICE “Alternatives to Detention” data published online by [Syracuse University’s Transaction Records Access Clearinghouse (TRAC)](https://trac.syr.edu/immigration/tools/).
