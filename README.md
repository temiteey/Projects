# Data Engineer Assessment Project
<!-- Data ETL with python and MySql (iterating through the keys and values in a dictionary, unpacking lists, renaming columns, resetting index) -->

  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Libraries Imported</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- Data Engineer Assessment Test-->
## About The Project

ETL on https://github.com/annexare/Countries/tree/master/data (Data source)
This project is targeted at performing ETL by iterating through  dictionaries with python and unpacking lists
It show cases Data wrangling capabilities, Extraction, Transformation and Loading of data from a json object.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Libraries Imported

Python libraries imported for this project include:

* import json
*import pandas as pd
*import numpy as np
*import mysql.connector as connection
*from sqlalchemy import create_engine
*import pymysql


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

An ETL workflow was created by reading the dataset into a Pandas DataFramethat brings the data into a MySQL database. 
Three(3) different tables were created named (continent, countries, and languages). 

Table Language  has 3 columns (language_code, name, native) which holds different languages spoken by different countries.
The primary key on the language table is language_code. column rtl was dropped for it has no significant impact on the other columns in the tble
and it is majorly filled with NAN. describe was caalled on the dataframe to make the decision to drop rtl.

Table continent holds 2 columns (continent_code and continent_name). On this table, the primary key is continent_code.

Table Countries  has 9 columns named(country_code, name,native,phone,continent,capital,currency,languages,code_3_letters).
This table has its primary key as country_code and it contains 2 foreign keys(languages & continent ).code_3_letters could also serve as a foreign key but
it is not needed in solving the etl challenge solved here.


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Temitope Ayinla - (linkedin.com/in/temitope-ayinla-2391b0195/) - ayinlatemitope.08@gmail.com

Project Link: [https://github.com/your_username/repo_name]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
I found these sites useful while working on this project

*pythontic.com/pandas/serialization/mysql#:~:text=Create%20a%20dataframe%20by%20calling,data%20from%20the%20pandas%20dataframe.
*[stackoverflow](https://stackoverflow.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
