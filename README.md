# US Politicians Twitter Dataset

 Dataset based on Twitter usernames of American politicians. Data extracted from Wikidata.
 
 Variables :

 1. Mandatory
    - ```Name```
    - ```Twitter_username```
    - ```Sex```
2. Optional
    - ```Account_start_time```
    - ```Account_ID```
    - ```Instagram_username```
    - ```Birthplace```
    - ```Political_party```
    - ~~Image~~

 The same politician can appear several times: if he has different pseudonyms on Twitter or Instagram, if he has been in several parties, or if several Twitter account IDs are associated with him. But the data is sorted in ascending order by name, so it is visible. See the [examples](https://github.com/W43GVG/US-Politicians-Twitter-Dataset#examples) part, where Julia Brownley is present twice.

# Examples
## JSON

[dataset.json](https://github.com/W43GVG/US-Politicians-Twitter-Dataset/blob/master/dataset.json)

```json
    {
        "Name": "Judy Chu",
        "Twitter_username": "RepJudyChu",
        "Account_start_time": "2010-09-22T00:00:00Z",
        "Account_ID": "193732179",
        "Sex": "female",
        "Birthplace": "United States of America",
        "Instagram_username": "repjudychu",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Julia Brownley",
        "Twitter_username": "RepBrownley",
        "Account_start_time": "2017-10-25T00:00:00Z",
        "Account_ID": "923251678652043269",
        "Sex": "female",
        "Birthplace": "United States of America",
        "Instagram_username": "juliabrownley26",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Julia Brownley",
        "Twitter_username": "RepBrownley",
        "Account_start_time": "2013-03-05T00:00:00Z",
        "Account_ID": "1243902714",
        "Sex": "female",
        "Birthplace": "United States of America",
        "Instagram_username": "juliabrownley26",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Julia Nesheiwat",
        "Twitter_username": "JuliaNesheiwat",
        "Sex": "female",
        "Birthplace": "United States of America",
        "Instagram_username": "julianesheiwat",
        "Political_party": "Republican Party"
    },
```
## CSV

[dataset.csv](https://github.com/W43GVG/US-Politicians-Twitter-Dataset/blob/master/dataset.csv)

| Name               | Twitter_username | Account_start_time   | Account_ID          | Sex    | Birthplace               | Instagram_username | Political_party  |
|--------------------|------------------|----------------------|---------------------|--------|--------------------------|--------------------|------------------|
| A. Donald McEachin | RepMcEachin      | 2017-01-03T00:00:00Z | 816181091673448448  | male   | Germany                  | repmceachin        | Democratic Party |
| Aaron Michlewitz   | RepMichlewitz    | 2010-06-27T00:00:00Z | 160246973           | male   | United States of America |                    | Democratic Party |
| Aaron Peskin       | AaronPeskin      | 2010-11-13T00:00:00Z | 215369273           | male   | United States of America | apeskin52          | Democratic Party |
| Aaron Peña         | AaronPena        | 2007-10-31T00:00:00Z | 9843332             | male   | United States of America |                    | Republican Party |
| Aaron Schock       | aaronschock      | 2009-03-12T00:00:00Z | 23951197            | male   | United States of America | aaronschock        | Republican Party |
| Abby Finkenauer    | Abby4Iowa        | 2013-03-12T00:00:00Z | 1262017122          | female | United States of America | abby4iowa          | Democratic Party |
| Abigail Spanberger | RepSpanberger    | 2018-12-28T00:00:00Z | 1078771401497161728 | female | United States of America | repspanberger      | Democratic Party |
| Abigail Spanberger | SpanbergerVA07   | 2018-12-28T00:00:00Z | 1078771401497161728 | female | United States of America | repspanberger      | Democratic Party | 
 
 CSV : 2591 rows.

# Changes
## November 17, 2020

 Added two variables:
 - Account_start_time
 - Account_ID

 Removed one variable:
 - Image

 Modified:
 - birth -> country of birth (```Birthplace```)

## Last update

 November 17, 2020.

W43GVG | Wikidata under  [CC0 1.0 Universal (CC0 1.0) Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)