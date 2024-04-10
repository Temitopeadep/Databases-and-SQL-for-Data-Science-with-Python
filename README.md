### Databases-and-SQL-for-Data-Science-with-Python

## Background
This project is final assignment for one of the 9 courses that needed to be passed for IBM Data Analyst Professional Certificate which is "Databases and SQL for Data Science with Python". All data used were provided IBM.

## Objective
The objective of this project is to answer 10 questions relating to Chicago crime rate, chicago census data and Chicago public schools data using SQL query

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

<img width="627" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/25e368ab-377e-43ae-8b79-a6b1c444cd8b">


Establish a connection between SQL magic module and the database FinalDB.db
<img width="404" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/2ef2f4a4-fb98-474f-8613-082c7bfdfde6">

# Problems
  1- Find the total number of crimes recorded in the CRIME table.
  
  <img width="484" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/0284c08e-decd-4d7f-a689-e10a3743dc39">
  
  2- List community area names and numbers with per capita income less than 11000

  <img width="578" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/ac5abb23-5ba4-45fe-be81-caed31d7073c">

  3- List all case numbers for crimes involving minors?(children are not considered minors for the purposes of crime analysis)

  <img width="554" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/be454e1b-ba8e-466e-b6b9-560e983513d5">

  4- List all kidnapping crimes involving a child?

  <img width="632" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/6c255495-9d9a-40ea-82d1-a3ad9c40df0c">

  5- List the kind of crimes that were recorded at schools. (No repetitions)

  <img width="586" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/3a390b5e-a735-4ba6-8f7f-1ecc379e6432">

  6- List the type of schools along with the average safety score for each type.

  <img width="497" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/5b310e63-2ac4-483c-92f0-e14051afbeed">

  7- List 5 community areas with highest % of households below poverty line

  <img width="518" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/d81ba659-8568-4ffc-9b63-90fbdca0f54f">
 
  8- Which community area is most crime prone? Display the coumminty area number only

  <img width="606" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/c3fc946a-d2fd-4c07-ab95-24398a2ef266">

  9- Use a sub-query to find the name of the community area with highest hardship index

  <img width="493" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/6f2d5878-6c24-4da9-a59e-1e1f3b0a68ca">

  10- Use a sub-query to determine the Community Area Name with most number of crimes?

  <img width="477" alt="image" src="https://github.com/Temitopeadep/Databases-and-SQL-for-Data-Science-with-Python/assets/142262047/d88e7a12-4dbc-4a47-9825-979d95d7e11a">









  





  







