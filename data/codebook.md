
#Codebook for data.csv

**File-Type:** CSV, 15 rows (+ 1 header), 13 column, N=1046

`data.csv` *is a processed form of the raw dataset: I aggregated passengers to age categories and only kept variables for victims and all passengers (seperated by men and women).*

## Variables

- **age_cat**: age categorie (ordinal) ["0 to 5", "6 to 10", ..., "70+]
- **m_died_pclass1**: number of 1st class male passengers who died (metric)
- **m_total_pclass1**: number of all 1st class male passengers (survived and died)
- **f_died_pclass1**: number of 1st class female passengers who died (metric)
- **f_total_pclass1**: number of all 1st class female passengers (survived and died)
- *... (same for 2nd and 3rd class)*

## Resources
[1] [Link to the raw dataset](http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/titanic3.csv)

[2] [Codebook of the raw dataset](http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/titanic3info.txt)