# SPED_DataScripts
Data dictionary

# Custom.SPED_All_Students_With_Disabilities

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| CUSTOMERNAME       | Varchar(100) | STATEID |             |       |
| SCHOOLNAME         | Varchar(100) | STATEID |             |       |
| STATEID            | Varchar(100) | STATEID |             |       |
| FIRSTNAME          | Varchar(100) | STATEID |             |       |
| LASTNAME           | Varchar(100) | STATEID |             |       |
| PRIMARYDISABILITY  | Varchar(100) | STATEID |             |       |
| BEGINDATE          | Datetime     | STATEID |             |       |
| SERVICE            | Varchar(100) | STATEID |             |       |
| EXTENDEDSCHOOLYEAR | Varchar(100) | STATEID |             |       |
| SERVICELOCATION    | Varchar(100) | STATEID |             |       |
| TIME               | Float        | STATEID |             |       |
| TIMEUNITS          | Varchar(100) | STATEID |             |       |
| TIMEFREQUENCY      | Varchar(100) | STATEID |             |       |
| LASTUPDATED        | Varchar(100) | STATEID |             |       |

#Custom.SPED_Custom_Screen

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| SYSTEMSTUDENTID       | Varchar(100) | SYSTEMSTUDENTID |             |       |
| SPED_NEXTANNUALIEP         | Varchar(100) | SYSTEMSTUDENTID |This is the IEP End Date field in the SLED report, which is 364 days after the IEP beginning date. Should be the same as the "IEP End" column in SEDS - reflects when it's due in SEDS             |       |
| SPED_PROJELIG            | Varchar(100) | SYSTEMSTUDENTID |             |       |
| SPED_TOTALHOURS          | Real | SYSTEMSTUDENTID |Represents ALL SPED hours (instruction support in Gen Ed and SPED settings, related services, and dedicated aide hours)             |       |
| SPED_FUNDING           | Varchar(100) | SYSTEMSTUDENTID |             |       |
| SPED_SPEDHOURS  | Real | SYSTEMSTUDENTID | Represents total SPED hours outside of Gen Ed setting (instructional support in SPED settings (pullout), related services)            |       |
| SPED_GENEDHOURS          | Real     | SYSTEMSTUDENTID |Represents total SPED hours inside of Gen Ed setting (instructional support in Gen Ed settings (push-in), related services)             |       |
| SPED_PERCENTOUTGENED            | Real | SYSTEMSTUDENTID |             |Total/32.5       |
| SPED_LRETIER | Varchar(100) | SYSTEMSTUDENTID |Tier A (80+% Gen Ed), Tier B (40-79% Gen Ed), Tier C (0-39% Gen Ed)               |Total/32.5     |
| SPED_SpInstSpEd    | Varchar(100) | SYSTEMSTUDENTID |Represents instructional support hours in SPED settings (not including related services)              |Kept in hours/week format       |
| SPED_SpInstGenEd               | Varchar(100)        | SYSTEMSTUDENTID |Represents instructional support hours in Gen Ed settings (not including related services)              |Kept in hours/week format       |
| SPED_DedicatedAideHrs          | Varchar(100) | SYSTEMSTUDENTID |             |       |
| SPED_Related_Behavior      | Varchar(100) | SYSTEMSTUDENTID |             |Keep in min/month format       |
| SPED_Related_Speech        | Varchar(100) | SYSTEMSTUDENTID |             |Keep in min/month format       |
| SPED_Related_OT          | Varchar(100) | SYSTEMSTUDENTID |             |Keep in min/month format       |
| SPED_Related_PT      | Varchar(100) | SYSTEMSTUDENTID |             |Keep in min/month format       |
| SPED_Related_Audiology        | Varchar(100) | SYSTEMSTUDENTID |             |Keep in min/month format       |

# Custom.SPED_Special_Education_Roster

| Field              | Type         | Key     | Description | Notes |
|--------------------|--------------|---------|-------------|-------|
| USI      | Varchar(100) | USI |             |       |
| FirstName         | Varchar(100) | USI |             |       |
| LastName            | Varchar(100) | USI |             |       |
| Gender          | Varchar(100) | USI |             |       |
| DateofBirth           | Date | USI |             |       |
| LEAname  | Varchar(100) | USI |             |       |
| LEAType          | Varchar(100)     | USI |             |       |
| SchoolName            | Varchar(100) | USI |             |       |
| SchoolType | Varchar(100) | USI |             |       |
| PrimaryDisability    | Varchar(100) | USI |             |       |
| IEPBeginDate               | Varchar(100)        | USI |             |       |
| IEPEndDate          | Varchar(100) | USI |             | 364 days after beginning date       |
| total_hours_out_of_gen_ed_setting      | Real | USI | Represents total SPED hours out of Gen Ed setting (instructional support in SPED settings (pullout), related services)            |       |
| total_hours_in_gen_ed_setting        | Real | USI | Represents total SPED hours inside of Gen Ed setting (instructional support in Gen Ed settings (push-in), related services)             |       |
| dedicated_aide_hours            | Real | USI |             |       |
| Total_Hours_Per_Week | Real | USI |Represents ALL SPED hours (instruction support in Gen Ed and SPED settings, related services, and dedicated aide hours)             |       |
| Special_Education_Level    | Varchar(100) | USI |             |       |
| Environment               | Varchar(2000)       | USI |Measures LRE Tier              |*Is 2000 a typo?     |
| EligibilityDate          | Varchar(200) | USI |             |       |
| ProjectedEligibilityDate      | Varchar(200) | USI |             |       |
| LastUpdated        | Varchar(100) | USI |             |       |
