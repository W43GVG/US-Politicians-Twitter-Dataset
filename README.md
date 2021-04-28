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
    - ```Facebook_ID```
    - ```Birthplace```
    - ```Birthday```
    - ```Age```
    - ```Political_party```
    - ~~Image~~

 The same politician can appear several times: if he has different pseudonyms on Twitter or Instagram, if he has been in several parties, or if several Twitter account IDs are associated with him. But the data is sorted in ascending order by name, so it is visible. See the [examples](https://github.com/W43GVG/US-Politicians-Twitter-Dataset#examples) part, where Julia Brownley is present twice.

# Examples

```
git clone https://github.com/W43GVG/US-Politicians-Twitter-Dataset
```

## JSON

```
wget https://raw.githubusercontent.com/W43GVG/US-Politicians-Twitter-Dataset/master/dataset.json
```

[dataset.json](https://github.com/W43GVG/US-Politicians-Twitter-Dataset/blob/master/dataset.json)

```json
    {
        "Name": "A. Donald McEachin",
        "Twitter_username": "RepMcEachin",
        "Twitter_account_start_time": "2017-01-03T00:00:00Z",
        "Account_ID": "816181091673448448",
        "Sex": "male",
        "Birthplace": "Germany",
        "birthday": "1961-10-10T00:00:00Z",
        "age": "59.0",
        "Instagram_username": "repmceachin",
        "Facebook_ID": "RepMcEachin",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Aaron Michlewitz",
        "Twitter_username": "RepMichlewitz",
        "Twitter_account_start_time": "2010-06-27T00:00:00Z",
        "Account_ID": "160246973",
        "Sex": "male",
        "Birthplace": "United States of America",
        "birthday": "1978-01-01T00:00:00Z",
        "age": "42.0",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Aaron Peskin",
        "Twitter_username": "AaronPeskin",
        "Twitter_account_start_time": "2010-11-13T00:00:00Z",
        "Account_ID": "215369273",
        "Sex": "male",
        "Birthplace": "United States of America",
        "birthday": "1964-06-17T00:00:00Z",
        "age": "56.0",
        "Instagram_username": "apeskin52",
        "Facebook_ID": "aaron.peskin",
        "Political_party": "Democratic Party"
    },
    {
        "Name": "Aaron Peña",
        "Twitter_username": "AaronPena",
        "Twitter_account_start_time": "2007-10-31T00:00:00Z",
        "Account_ID": "9843332",
        "Sex": "male",
        "Birthplace": "United States of America",
        "birthday": "1959-06-08T00:00:00Z",
        "age": "61.0",
        "Political_party": "Republican Party"
    },
```

## CSV

```
wget https://raw.githubusercontent.com/W43GVG/US-Politicians-Twitter-Dataset/master/dataset.csv
```

[dataset.csv](https://github.com/W43GVG/US-Politicians-Twitter-Dataset/blob/master/dataset.csv)

| Name               | Twitter_username | Twitter_account_start_time | Account_ID          | Sex    | Birthplace               | birthday             | age  | Instagram_username | Facebook_ID       | Political_party  |
|--------------------|------------------|----------------------------|---------------------|--------|--------------------------|----------------------|------|--------------------|-------------------|------------------|
| A. Donald McEachin | RepMcEachin      | 2017-01-03T00:00:00Z       | 816181091673448448  | male   | Germany                  | 1961-10-10T00:00:00Z | 59.0 | repmceachin        | RepMcEachin       | Democratic Party |
| Aaron Michlewitz   | RepMichlewitz    | 2010-06-27T00:00:00Z       | 160246973           | male   | United States of America | 1978-01-01T00:00:00Z | 42.0 |                    |                   | Democratic Party |
| Aaron Peskin       | AaronPeskin      | 2010-11-13T00:00:00Z       | 215369273           | male   | United States of America | 1964-06-17T00:00:00Z | 56.0 | apeskin52          | aaron.peskin      | Democratic Party |
| Aaron Peña         | AaronPena        | 2007-10-31T00:00:00Z       | 9843332             | male   | United States of America | 1959-06-08T00:00:00Z | 61.0 |                    |                   | Republican Party |
| Aaron Schock       | aaronschock      | 2009-03-12T00:00:00Z       | 23951197            | male   | United States of America | 1981-05-28T00:00:00Z | 39.0 | aaronschock        |                   | Republican Party |
| Abby Finkenauer    | Abby4Iowa        | 2013-03-12T00:00:00Z       | 1262017122          | female | United States of America | 1988-12-27T00:00:00Z | 31.0 | abby4iowa          | RepAbbyFinkenauer | Democratic Party |
| Abigail Spanberger | SpanbergerVA07   | 2018-12-28T00:00:00Z       | 1078771401497161728 | female | United States of America | 1978-08-01T00:00:00Z | 42.0 | repspanberger      | RepSpanberger     | Democratic Party |
| Abigail Spanberger | RepSpanberger    | 2018-12-28T00:00:00Z       | 1078771401497161728 | female | United States of America | 1978-08-01T00:00:00Z | 42.0 | repspanberger      | RepSpanberger     | Democratic Party |

 CSV : 2964 rows.

# Changes
## February 5, 2021

 Refining the results (e.g., removal of politicians who are American but practising in other countries).

 Added one variable:
 - ```Facebook_ID```

 Modified:
 - ```Account_start_time``` -> ```Twitter_account_start_time```

## November 29, 2020

 Refining the results (e.g., removal of politicians who are American but practising in other countries).

## November 17, 2020  (2)

 Added two variables:
 - ```Birthday```
 - ```Age```

 Refining the results (e.g., removal of politicians who are American but practising in other countries).

## November 17, 2020

 Added two variables:
 - ```Account_start_time```
 - ```Account_ID```

 Removed one variable:
 - ```Image```

 Modified:
 - ```birth``` -> country of birth (```Birthplace```)

## Last update

 February 5, 2020.

# External uses

This datased has been ported to [Kaggle](https://www.kaggle.com/mrmorj/us-politicians-twitter-dataset) (not by me).

It was used for building this [dataset](https://www.kaggle.com/jeevanbhoot/tweets-from-us-politicians).

# License, notes

W43GVG | Wikidata under  [CC0 1.0 Universal (CC0 1.0) Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)

Note that the data is extracted from Wikidata, so there may be errors. In case of errors, it is preferable to correct it directly on Wikidata, so it will be corrected in the dataset in the next update.