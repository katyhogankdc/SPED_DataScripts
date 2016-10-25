# SPED_DataScripts
Data dictionary

# Custom.SPED_All_Students_With_Disabilities

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| CUSTOMERNAME       | Varchar(100) | Primary Key |             |       |
| SCHOOLNAME         | Varchar(100) |  |             |       |
| STATEID            | Varchar(100) |  |             |       |
| FIRSTNAME          | Varchar(100) |  |             |       |
| LASTNAME           | Varchar(100) |  |             |       |
| PRIMARYDISABILITY  | Varchar(100) |  |             |       |
| BEGINDATE          | Datetime     |  |             |       |
| SERVICE            | Varchar(100) |  |             |       |
| EXTENDEDSCHOOLYEAR | Varchar(100) |  |             |       |
| SERVICELOCATION    | Varchar(100) |  |             |       |
| TIME               | Float        |  |             |       |
| TIMEUNITS          | Varchar(100) |  |             |       |
| TIMEFREQUENCY      | Varchar(100) |  |             |       |
| LASTUPDATED        | Varchar(100) |  |             |       |

#Custom.SPED_Custom_Screen

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| SYSTEMSTUDENTID       | Varchar(100) | Primary Key |             |       |
| SPED_NEXTANNUALIEP         | Varchar(100) |  |This is the IEP End Date field in the SLED report, which is 364 days after the IEP beginning date. Should be the same as the "IEP End" column in SEDS - reflects when it's due in SEDS             |       |
| SPED_PROJELIG            | Varchar(100) |  |             |       |
| SPED_TOTALHOURS          | Real |  |Represents ALL SPED hours (instruction support in Gen Ed and SPED settings, related services, and dedicated aide hours)             |       |
| SPED_FUNDING           | Varchar(100) |  |             |       |
| SPED_SPEDHOURS  | Real |  | Represents total SPED hours outside of Gen Ed setting (instructional support in SPED settings (pullout), related services)            |       |
| SPED_GENEDHOURS          | Real     |  |Represents total SPED hours inside of Gen Ed setting (instructional support in Gen Ed settings (push-in), related services)             |       |
| SPED_PERCENTOUTGENED            | Real |  |             |Total/32.5       |
| SPED_LRETIER | Varchar(100) |  |Tier A (80+% Gen Ed), Tier B (40-79% Gen Ed), Tier C (0-39% Gen Ed)               |Total/32.5     |
| SPED_SpInstSpEd    | Varchar(100) |  |Represents instructional support hours in SPED settings (not including related services)              |Kept in hours/week format       |
| SPED_SpInstGenEd               | Varchar(100)        |  |Represents instructional support hours in Gen Ed settings (not including related services)              |Kept in hours/week format       |
| SPED_DedicatedAideHrs          | Varchar(100) |  |             |       |
| SPED_Related_Behavior      | Varchar(100) |  |             |Keep in min/month format       |
| SPED_Related_Speech        | Varchar(100) |  |             |Keep in min/month format       |
| SPED_Related_OT          | Varchar(100) |  |             |Keep in min/month format       |
| SPED_Related_PT      | Varchar(100) |  |             |Keep in min/month format       |
| SPED_Related_Audiology        | Varchar(100) |  |             |Keep in min/month format       |

# Custom.SPED_Special_Education_Roster

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| USI      | Varchar(100) | Primary Key |             |       |
| FirstName         | Varchar(100) |  |             |       |
| LastName            | Varchar(100) |  |             |       |
| Gender          | Varchar(100) |  |             |       |
| DateofBirth           | Date |  |             |       |
| LEAname  | Varchar(100) |  |             |       |
| LEAType          | Varchar(100)     |  |             |       |
| SchoolName            | Varchar(100) |  |             |       |
| SchoolType | Varchar(100) |  |             |       |
| PrimaryDisability    | Varchar(100) |  |             |       |
| IEPBeginDate               | Varchar(100)        |  |             |       |
| IEPEndDate          | Varchar(100) |  |             | 364 days after beginning date       |
| total_hours_out_of_gen_ed_setting      | Real |  | Represents total SPED hours out of Gen Ed setting (instructional support in SPED settings (pullout), related services)            |       |
| total_hours_in_gen_ed_setting        | Real |  | Represents total SPED hours inside of Gen Ed setting (instructional support in Gen Ed settings (push-in), related services)             |       |
| dedicated_aide_hours            | Real |  |             |       |
| Total_Hours_Per_Week | Real |  |Represents ALL SPED hours (instruction support in Gen Ed and SPED settings, related services, and dedicated aide hours)             |       |
| Special_Education_Level    | Varchar(100) |  |             |       |
| Environment               | Varchar(2000)       |  |Measures LRE Tier              |*Is 2000 a typo?     |
| EligibilityDate          | Varchar(200) |  |             |       |
| ProjectedEligibilityDate      | Varchar(200) |  |             |       |
| LastUpdated        | Varchar(100) |  |             |       |
