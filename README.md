<a name="readme-top"></a>

# NYC Arrests Analysis

<details open>
<summary>Table of Contents</summary>
<ol>
  <li>
    <a href="#introduction">Introduction</a>
  </li>
  <li>
    <a href="#dataset-used">Dataset Used</a>
  </li>
  <li>
    <a href="#libraries">Libraries</a>
  </li>
  <li>
    <a href="#further-detail">Further Detail</a>
  </li>
  <li>
    <a href="#license">License</a>
  </li>
</ol>
</details>

## Introduction
This project was made for the Computer Science 3225 Class Data Tools and Algorithms at Brooklyn College, taught by Professor Matthew Mcneill, the project aims to create a portfolio level analysis project aimed at having us use real world analytical techniques taught in class.

## Dataset Used
The dataset I chose to do complex analysis on was the NYC Arrests year to date Dataset provided on NYC Open data:
- Dataset Link: [Arrests Dataset](https://data.cityofnewyork.us/Public-Safety/NYPD-Arrest-Data-Year-to-Date-/uip8-fykc/about_data)
- The dataset has the following column format:

    | Column Name          | Description                                                                  | API Field Name    | Data Type      |
    |----------------------|------------------------------------------------------------------------------|-------------------|----------------|
    | ARREST_KEY           | Randomly generated persistent ID for each arrest                               | arrest_key        | Text           |
    | ARREST_DATE          | Exact date of arrest for the reported event                                  | arrest_date       | Floating Timestamp |
    | PD_CD                | Three digit internal classification code (more granular than Key code)         | pd_cd             | Number         |
    | PD_DESC              | Description of internal classification corresponding with PD code (more granular than Offense description) | pd_desc           | Text           |
    | KY_CD                | Three digit internal classification code (more general category than PD code)    | ky_cd             | Number         |
    | OFNS_DESC            | Description of internal classification corresponding with KY code (more general category than PD description) | ofns_desc         | Text           |
    | LAW_CODE             | Law code corresponds to the New York State Penal Law, VTL and other various local laws | law_code          | Text           |
    | LAW_CAT_CD           | Level of offense: felony, misdemeanor, violation                             | law_cat_cd        | Text           |
    | ARREST_BORO          | Borough of arrest. B(Bronx), S(Staten Island), K(Brooklyn), M(Manhattan), Q(Queens) | arrest_boro       | Text           |
    | ARREST_PRECINCT      | Precinct where the arrest occurred                                           | arrest_precinct   | Number         |
    | JURISDICTION_CODE    | Jurisdiction responsible for arrest. Jurisdiction codes (typically 0 (Transit) and 20 (Housing)) represent NYPD whilst codes 1 and 2 represent non NYPD Jurisdictions | jurisdiction_code | Number         |
    | AGE_GROUP            | Perpetrator's age within a category                                          | age_group         | Text           |
    | PERP_SEX             | Perpetrator's sex description                                                | perp_sex          | Text           |
    | PERP_RACE            | Perpetrator's race description                                               | perp_race         | Text           |
    | X_COORD_CD           | Midblock X-coordinate for New York State Plane Coordinate System, Long Island Zone, NAD 83, units feet (FIPS 3104) | x_coord_cd        | Number         |
    | Y_COORD_CD           | Midblock Y-coordinate for New York State Plane Coordinate System, Long Island Zone, NAD 83, units feet (FIPS 3104) | y_coord_cd        | Number         |
    | Latitude             | Latitude coordinate for Global Coordinate System, WGS 1984, decimal degrees (EPSG 4326) | latitude          | Number         |
    | Longitude            | Longitude coordinate for Global Coordinate System, WGS 1984, decimal degrees (EPSG 4326) | longitude         | Number         |
    | New Georeferenced Column |                                                                              | geocoded_column   | Point          |

## Libraries
The libraries used here will be listed under:

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Further Detail
Further detail to the assignment such as methods, hypothesis, questions, and so on will be provided as links here:
- Report Link: TBD

## Special Thanks
Special thanks to NYC Open Data for providing the people with free access to datasets, it is great help to young analysts who wish to do work on important datasets.
- NYC Open Data: [Homepage](https://opendata.cityofnewyork.us/)

    <img src="https://opendata.cityofnewyork.us/wp-content/themes/opendata-wp/assets/img/nyc-open-data-logo.svg" alt='nyc open data' width=200>

## License
MIT License

Copyright (c) 2025 David Rodriguez

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[Python]: https://img.shields.io/badge/python-FFDE57?style=for-the-badge&logo=python&logoColor=4584B6
[Python-url]: https://www.python.org/