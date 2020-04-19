# Bike theft in Berlin

### Objective

This project entails the analysis of the data regarding bike thefts in Berlin from 2012 to 2019. 

### Data acquisition and wrangling

The data was obtained from the Kriminalitätsatlas Berlin (https://www.kriminalitaetsatlas.berlin.de/K-Atlas/atlas.html), which publishes the  total reported cases and the frequency per 100,000 inhabitants of a series of crimes that were reported to the police in the aforementioned period of time.

The data is presented per districts (Bezirke), district regions (Bezirkesregionen) and a key identifier for each district region (Lebensweltlich orientierten Räume "LOR"). However, none of the three parameters are identified by Tableau as a Geographic Role. 

In order to associate the obtained data to geografic points, the LOR keys were associated to a number of locations that was obtained from the Senatsverwaltung für Stadtentwicklung und Wohnen webpage (https://www.stadtentwicklung.berlin.de/planen/basisdaten_stadtentwicklung/lor/de/download.shtml). 

A post code was associated to each district region manually, which was then added to the tabular data for the visualization in a map.  

Morever, bar plots are presented for the total count and frequency of cases per 100,000 inhabitants per district and per district region per year. Line plots are also presented to see the changes in the total number of cases over the years for the district regions.

The following files can be found in the "Data" folder of this repository:

1. "Fallzahlen&HZ 2012-2019.xlsx" in the "Kriminalitätsatlas" folder. This is the raw data from the Kriminalitätsatlas Berlin.
2. "LOR-Schluesselsystematik_2019.xls" in the "LOR" folder. This is the data with the associated LOR keys to district, district regions and a number of locations. 
3. "Falle_KA.xlsx" in the "Clean" folder. This is the arranged data for total cases with associated post codes to district regions, which were found and manually to the existing data. 
4. "HZ_KA.xlsx" in the "Clean" folder. This This is the arranged data for the frequency of cases with associated post codes to district regions, which were found and manually to the existing data. The data of the bike thefts was then added as a column to the "Falle_KA.xlsx" file.

The results of the analysis are presented in the Tableau Packaged Workbook named "Bike theft in Berlin" in this folder.

