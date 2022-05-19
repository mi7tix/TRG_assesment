Overview
========

Current assesment based on https://data.police.uk/data/ and
executed with Jupite notebook as a bas driver for pyspark
`spark-3.2.1-bin-hadoop3.2`


Required files
======================

* `asses/` - source data directory
* `assesment.ipynb` - Jupiter notebook with a analytics steps


Task Steps
==========

1. Read the data from `asses` folder , split datasets by streets and outcomes titles, 
select proper related to the crime statistics.
`input_file_name` used to parse filenames for the `DistrictName` field

2. We crop all the path data from the filenames and leave only disricts. Join `outcomes`
 and `street` Dataframes by `CrimeId` fields. 

3. Provide KPI statistics for `districtName`, `crimeType` and `lastOutcomeCategory`


