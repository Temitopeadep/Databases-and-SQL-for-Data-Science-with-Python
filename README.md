### Databases-and-SQL-for-Data-Science-with-Python

## Background
This project is final assignment for one of the course(Databases and SQL dor Data Science with Python) that need to be passed for IBM Data analyst Professional Certificate.
All data used were provided IBM. Ten problems need to be solved using SQLite with Python)

## Introduction
  - Understand three Chicago datasets

  - Load the three datasets into three tables in a SQLIte database

  - Execute SQL queries to answer assignment questions
## Understand the datasets
To complete the assignment problems in this notebook you will be using three datasets that are available on the city of Chicago's Data Portal:
 
  - Socioeconomic Indicators in Chicago
This dataset contains a selection of six socioeconomic indicators of public health significance and a “hardship index,” for each Chicago community area, for the years 2008 – 2012.
A detailed description of this dataset and the original dataset can be obtained from the Chicago Data Portal at [link](https://data.cityofchicago.org/Health-Human-Services/Census-Data-Selected-socioeconomic-indicators-in-C/kn9c-c2s2/about_data?cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork-20127838&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvo_campaign=000026UJ&cvosrc=email.Newsletter.M12345678&utm_content=000026UJ&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2021-01-01&utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_term=10006555)

  -  Chicago Public Schools
This dataset shows all school level performance data used to create CPS School Report Cards for the 2011-2012 school year. This dataset is provided by the city of Chicago's Data Portal.
A detailed description of this dataset and the original dataset can be obtained from the Chicago Data Portal at [link](https://data.cityofchicago.org/Education/Chicago-Public-Schools-Progress-Report-Cards-2011-/9xs2-f89t/about_data?cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork-20127838&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvo_campaign=000026UJ&cvosrc=email.Newsletter.M12345678&utm_content=000026UJ&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2021-01-01&utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_term=10006555)

  - Chicago Crime Data
This dataset reflects reported incidents of crime (with the exception of murders where data exists for each victim) that occurred in the City of Chicago from 2001 to present, minus the most recent seven days.
A detailed description of this dataset and the original dataset can be obtained from the Chicago Data Portal at [link](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/about_data?cm_mmc=Email_Newsletter-_-Developer_Ed%2BTech-_-WW_WW-_-SkillsNetwork-Courses-IBMDeveloperSkillsNetwork-DB0201EN-SkillsNetwork-20127838&cm_mmca1=000026UJ&cm_mmca2=10006555&cm_mmca3=M12345678&cvo_campaign=000026UJ&cvosrc=email.Newsletter.M12345678&utm_content=000026UJ&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDB0201ENSkillsNetwork20127838-2021-01-01&utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_term=10006555)


# Store the datasets in database tables
To analyze the data using SQL, it first needs to be loaded into SQLite DB. We will create three tables in as under
  - CENSUS_DATA
  - CHICAGO_PUBLIC_SCHOOLS
  - CHICAGO_CRIME_DATA
Load the pandas and sqlite3 libraries and establish a connection to FinalDB.db
<img width="620" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/2fb4a4cf-dc19-4490-b994-686967635d68">
Establish a connection between SQL magic module and the database FinalDB.db
<img width="404" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/2ef2f4a4-fb98-474f-8613-082c7bfdfde6">







