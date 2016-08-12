## WIKI --> https://github.com/TDahlberg/nonprofit_data/wiki

This repository contains a dataset that when unzipped, contains every single IRS registered nonprofit (~1.5 million) in the united states. Why might you want to use this file for analysis over the IRS version? It's geocoded, so almost every single one of the 1.5 million or so records has a latitude / longitude for mapping. Descriptive NTEE codes were also added in, so users wouldn't need to cross reference the NTEE codes with a metadata document.

# Sources
List of nonprofits downloaded from [https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf](https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf)

NTEE codes downloaded from [http://nccs.urban.org/classification/ntee.cfm](http://nccs.urban.org/classification/ntee.cfm)

# File Contents:
This repository contains two sets of files:
* Every Nonprofit in the United States (1.5 million +) as a 4-part .ZIP file
  * all_nonprofits.csv.zip.001
  * all_nonprofits.csv.zip.002
  * all_nonprofits.csv.zip.003
  * all_nonprofits.csv.zip.004
* NTEE codes and definitions 
  * ntee_codes.csv 

### How to get the data:
 1. Download this repository by clicking "Clone or Download" on the right side
   2. Select "Download ZIP"
 2. Open the folder, and unzip "all_nonprofits.csv.zip.001". This will unzip all four files into one CSV file.
 3. Voila, the 300mb+ CSV includes every single nonprofit in the US. Refer to the [Wiki](https://github.com/TDahlberg/nonprofit_data/wiki) for field definitions and metadata. 


### Data processing:
* Geocoded and added latitude / longitude [Mapadelphia](https://www.twitter.com/mapadelphia)
* Merged shapefiles ([Mapadelphia](www.twitter.com/mapadelphia))
* Output to CSV
* Cleaned NTEE codes into a CSV
* Joined NTEE codes, more detailed descriptions to nonprofit list
* Removed category header.
 
### Working with the data:
I recommend using Python + Pandas, R, or SQL, as the final 300mb+ file is much too large for standard spreadsheet software. Maybe start with [this Python notebook](https://gist.github.com/TDahlberg/b6b595c6d5d23036e07907dc9184d486) for ideas?
