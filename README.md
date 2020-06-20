# problem 4
# metadata
This is accidental drug related deaths from 2012-2018 from https://catalog.data.gov/dataset/accidental-drug-related-deaths-january-2012-sept-2015
| Column Name | Description |
| ------- | ------- |
| Date	| The year (4 digits), month (2 digits), and (day of the month) followed by a space then the hour (two digit) |
| Date Type |	Whether if it is the date of death or date of the incident being reported |
| Race	| Ethnic background of the individual |
| Residence County	| What city the individual resided in |
| Residence State	| What state the individual resided in  |
| Death City	|  The city the individual was pronounced dead in |
| Death County | The county the individual was pronounced dead in |	
| Location	| Where exactly the individual died (home, hospital, etc) |
| Location if other| Where exactly the individual died (home, hospital, etc) |
| Description of Injury | What caused the death |
| Injury Place | Where exactly the individual had the incident in (home, hotel, etc) |
| Injury City | City where the individual got injured in |
 | Injury State | State where the individual got injured in |
 | COD | Cause of death |
 | Sex | birth gender of the individual |
 
# How I Would Normalize
 I would have one table simply with age, sex, race, death county, location, description of injury, and COD.
 
 This table will represent the data in a more concise way that simply gives background information, geographical location, where they died to see if they had gotten treatment, and the exact cause of death.
 
 # The data for colomn
 Column | Type
--- | ---
Age | CHAR string (2 digits)
Sex | VARCHAR string (max 200 characters)
Race | VARCHAR string (max 10 characters)
Death County| VARCHAR string (max 10 characters)
Location | VARCHAR string (max 10 characters)
DOI | DATETIME 
COD | VARCHAR string (max 10 charcters)
