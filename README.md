# US Politicians Twitter Dataset
 Dataset based on usernames of American politicians. Data extracted from Wikidata.
 
 Variables : 
 1. Mandatory

    a. Name

    b. Twitter username

    c. Sex

    d. Birth

2. Optional

    a. Instagram
    
    b. Political party
    
    c. Image
 The same politician can appear several times: if he has different pseudonyms on Twitter or Instagram, if he has been in several parties, or if several photos are associated with him. But the data is sorted in ascending order by name, so it is visible. See the "example" part, where José Enrique Serrano is present twice.

# Example
```json
    {
        "Name": "José Enrique Serrano",
        "Twitter username": "RepJoseSerrano",
        "Sex": "male",
        "Birth": "Mayagüez",
        "Instagram": "repjoseserrano",
        "Political party": "Democratic Party",
        "Image": "http://commons.wikimedia.org/wiki/Special:FilePath/Jose%20Serrano%2C%20official%20109th%20Congress%20photo.jpg"
    },
    {
        "Name": "José Enrique Serrano",
        "Twitter username": "RepJoseSerrano",
        "Sex": "male",
        "Birth": "Mayagüez",
        "Instagram": "repjoseserrano",
        "Political party": "Democratic Party",
        "Image": "http://commons.wikimedia.org/wiki/Special:FilePath/Josieserrano.jpeg"
    },
    {
        "Name": "José R. Oliva",
        "Twitter username": "repjoseoliva",
        "Sex": "male",
        "Birth": "Elizabeth",
        "Political party": "Republican Party",
        "Image": "http://commons.wikimedia.org/wiki/Special:FilePath/Jose%20R.%20Oliva.jpg"
    },
    {
        "Name": "José R. Rodríguez",
        "Twitter username": "JoseforTexas",
        "Sex": "male",
        "Birth": "Alice",
        "Political party": "Democratic Party"
    },
```

 CSV : 2247 rows.
 Last update: November 16, 2020.


W43GVG | Wikidata under  [CC0 1.0 Universal (CC0 1.0) Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/)