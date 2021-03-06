# MLS Salaries
Major League Soccer players salaries from 2007 until 2015 :
+ Source : [Major League Soccer Players Union website](https://www.mlsplayers.org/salary_info.html)
+ Raw data extracted from pdf files with [Tabula](http://tabula.technology/)
+ Cleaned with [OpenRefine](http://openrefine.org/) and Excel

## Available Files :
There are 2 tables available: salaries and mlsTeams.
You can join the **_SalaryShortClub_** field from the salaries table with the **_Short_** field present in the mlsTeams table.

### Salaries
+ [salaries.csv](https://github.com/alexmille/DataSets/blob/master/MLS-Salaries/salaries.csv)
+ [salaries.json](https://github.com/alexmille/DataSets/blob/master/MLS-Salaries/salaries.json)

**Example :**

|Header              |Example           |Description                                                           |
|--------------------|------------------|----------------------------------------------------------------------|
|SalaryShortClub     |SEA               |Team (Seattle in example). **Foreign Key** (PK in **mlsTeams** table) |
|SalaryLastName      |Doe               |Last Name                                                             |
|SalaryFirstName     |John              |First Name                                                            |
|SalaryName          |John Doe          |First & Last Name concatenated                                        |
|SalaryPos           |GK                |Position (goalkeeper in example)                                      |
|SalaryBaseSalary    |200000.00         |Annual salary (in USD)                                                |
|SalaryCompensation  |250000.00         |Annual salary including annualized bonuses (in USD)    |
|SalaryDate          |July 10, 2008     |                                                                      |
|SalaryYear          |2008              |                                                                      |
|SalaryMonth         |July              |                                                                      |
|SalaryMonthYear     |Jul-08            |                                                                      |
|Designated Player   |Designated Player |Acts as a flag. Blank if not a designated player                      |
|Remarks             |                  |Additional information                                                |

Salaries are available for the following years and months :

|Year  |	Quarter |	Month|
|------|----------|------|
|2007	|Q3	    | July
|2008	|Q3 | July
|2009	|Q3	|September
|2010	|Q3	|August
|2011	|Q1	|January
|2012	|Q1	|January
|2012	|Q2	|May
|2012	|Q3	|August
|2013	|Q2	|May
|2013	|Q3	|August
|2013	|Q3	|September
|2014	|Q2	|April
|2014	|Q3	|September
|2015	|Q3	|September

### Teams
+ [mlsTeams.csv](https://github.com/alexmille/DataSets/blob/master/MLS-Salaries/mlsTeams.csv)
+ [mlsTeams.json](https://github.com/alexmille/DataSets/blob/master/MLS-Salaries/mlsTeams.json)

**Example :**

|Header              |Example           |Description                                                           |
|--------------------|------------------|----------------------------------------------------------------------|
|Short               |CHV               |Team (Chivas in example). **Primary Key** (FK in **salaries** table)  |
|Team                |Chivas USA        |Team Full Name                                                        |
|City                |Carson            |Where are they playing ?                                              |
|State               |California        |In which State ?                                                      |
|Country             |USA               |US or Canada ?                                                        |
|Stadium             |StubHub Center    |Current Stadium                                                       |
|StadiumLatitude     |33.8643414        |Stadium Latitude                                                      |
|StadiumLongitude    |-118.2611082      |Stadium Longitude (but you guessed it, didn't you ?)                  |
|Conference          |Western Conference|East side Vs West side                                                |
|Joined              |2005              |When did this team joined the League ?                                |
|Active              |N                 |Is this team still active ? Y for yes, N for no                       |
|Defunct             |2014              |This team ceased to exist that year                                   |



## Quick Facts
(*source wikipedia*)
* MLS began play in **1996** with **10 teams**
* The **first game** was held on **April 6, 1996**, as the San Jose Clash defeated D.C. United
* Major League Soccer's **regular season** runs from **March to October**
* The Supporters' Shield is an annual award given to the Major League Soccer team with the best regular season record, as determined by the MLS points system
* The MLS regular season is followed by the 12-team MLS Cup Playoffs in November, ending with the MLS Cup championship final in early December
* Teams are divided into the Eastern and Western Conferences
