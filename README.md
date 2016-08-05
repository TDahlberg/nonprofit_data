# WIKI --> https://github.com/TDahlberg/nonprofit_data/wiki

# NTEE Codes
List of Nonprofits downloaded from [https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf](https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf)

Codes downloaded from [http://nccs.urban.org/classification/ntee.cfm](http://nccs.urban.org/classification/ntee.cfm)

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


### Steps taken:
 * Added new category field.
 * Removed category header. 
 * Converted to CSV.
 * Geocoded and added latitude / longitude

### Working with the data:
I recommend using Python + Pandas, R, or SQL, as the final 300mb+ file is much too large for standard spreadsheet software. Maybe start with [this Python notebook](https://gist.github.com/TDahlberg/b6b595c6d5d23036e07907dc9184d486)?
