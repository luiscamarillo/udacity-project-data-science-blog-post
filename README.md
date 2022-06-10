# Analyzing the 2021 and 2018 Mexican Chamber of Deputies elections

This project is a part of Udacity's Data Science Nanodegree, where I analyze the results of the 2021 and 2018 Mexican legislative elections with the purpose of effectively communicating technical results.
## Installations
This jupyter notebook can be installed through anaconda and was written in python 3.10.4.
It requires the following packages:
- pandas
- numpy
- seaborn
- matplotlib
- geopandas

The datasets with election results and candidates were downloaded from the official website of the National Electoral Institute (INE): [2018 results](https://computos2018.ine.mx/#/diputaciones/nacional/1/3/1/1), [2021 results](https://computos2021.ine.mx/votos-distrito/mapa). In addition, I downloaded a shape file for the map of the country's territorial divisions from the [CONABIO](http://www.conabio.gob.mx/informacion/metadata/gis/destdv250k_2gw.xml?_xsl=/db/metadata/xsl/fgdc_html.xsl&_indent=no).

## Project Motivation
For this project, I will be analyzing the results of the 2021 Mexican legislative midterm election for the 300 Chamber of Deputies districts, and comparing the outcome with the 2018 Mexican federal election.

I am personally very interested in elections worldwide and am an avid follower of election twitter, a community that analyzes and maps elections around the globe. With the recent gubernatorial elections of June 2022 here in Mexico and a lot of talk about a united opposition confronting Morena's electoral prowess in the presidential election of 2024, I thought it would be fun to analyze the past two federal results for the Chamber of Deputies.
The project follows the CRISP-DM Data Science process:

### Business Understanding

Mexico uses a mixed-member majoritarian system to elect the 500 members of the lower house of the Congress of the Union: **300 members competing in individual districts using a first-past-the-post electoral system**, and another 200 elected through proportional representation from five regional constituencies. 

**The purpose of this project is to answer the following three questions as related to the election results:**

1. What would have happened if all four opposition parties ran together against Morena in every one of the 300 FTPT districts?
2. In which states did Morena lose or gain support in 2021 compared to the 2018 Chamber of Deputies election?
3. Did parties benefit in 2021 from the new reelection rules by renominating incumbents compared to their results in open seats?

### Data Understanding
Importing the datasets, inspecting the data for missing values, presenting descriptive statistics, visualizing distributions

### Data Preparation
Cleaning data, aggregating results, and creating dataframes with coalitions running per district, coalitions shared results, and final winner as basis for further analysis/evaluation.

### Evaluation of Results
Analyzing and visualizing data, and presenting answers and conclusions re: the business questions.
## File Descriptions
- Mexican_legislative_elections.ipynb - Jupyter Notebook with analysis
- data/2018/diputaciones.csv - contains 2018 Chamber of Deputy results
- data/2018/diputaciones_candidaturas_2018.csv - contains 2018 Chamber of Deputy candidates
- data/2021/diputaciones.csv - contains 2021 Chamber of Deputy results
- data/2021/diputaciones_candidaturas_2021.csv - contains 2021 Chamber of Deputy candidates
- data/Maps/destdv250k_2gw.shp - Map of Mexico's territorial divisions shape file

## Results & Improvements
The results can be found in the following [Medium blog post](https://medium.com/@luiscamarillo97/can-morenas-electoral-machine-be-stopped-896d3cfda6e7).

## Licensing & Acknowledgements
Feel free to reuse this code under the MIT License. Special thanks to the INE and CONABIO for the datasets used.
