# eDNA

Code for converting a test eDNA data set (18S Monterey Bay Time Series data, Plate S, from Francisco Chavez's group) to [Darwin Core Standard format](https://dwc.tdwg.org/terms/#occurrence). The conversion follows GBIF's [guide to publishing DNA-derived biodiversity data](https://docs.gbif.org/publishing-dna-derived-data/1.0/en/).

Author: Diana LaScala-Gruenewald <br>
Language: Python 3.7

## Folders and files currently included

### OBIS_data - practice data for conversion
- **eDNA_practice_conversion.ipynb** - Jupyter notebook containing initial code for DwC conversion
- **eDNA_practice_conversion_draft2.ipynb** - Jupyter notebook containing second draft of code for DwC conversion, where I took an initial stab at handling non-Linnaean species names
- **eDNA_practice_conversion_draft3.ipynb** - Jupyter notebook containing third draft of code for DwC conversion, where I attempt to match all taxa on [WoRMS](http://www.marinespecies.org/) at the lowest possible taxonomic rank
- **eDNA_practice_conversion_draft4.ipynb** - Jupyter notebook containing final code for DwC conversion, with the names of each taxon matched on both WoRMS and the [NCBI taxonomy database](https://www.ncbi.nlm.nih.gov/taxonomy), and with occurrence and [DNA-derived extension](https://tools.gbif.org/dwca-validator/extension.do?id=http://rs.gbif.org/terms/1.0/DNADerivedData) files separated
- **eDNA_use_case** - CSV data tables and Python code currently in development for a use case on the IOOS GitHub 

### WoRMS.py

Python module containing functions for querying the [World Register of Marine Species (WoRMS) REST API](http://www.marinespecies.org/rest/).

## Links to completed archives

[OBIS](https://obis.org/dataset/62b97724-da17-4ca7-9b26-b2a22aeaab51) <br>
[GBIF](https://www.gbif.org/dataset/e0b59ee7-19ae-4eb0-9217-33317fb50d47)
