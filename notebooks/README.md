# Exploratory Notebooks

## Carpentries_lesson.ipynb

Began explorations with some code from the Carpentries lesson 
[Carpentries: Frictionless Data for Agriculture](https://carpentries-incubator.github.io/frictionless-data-agriculture/03-frictionless-tables/index.html). 
It automatically generates the schema from the input CSV file.

- Input: capacity.csv
- Output: test_schema.json


## make_package.ipynb

Explored altering fields, adding information, printing the output to screen, and automatically validating it.

- Input: capacity.csv
- Output: test_datapackage.json

## try_oemetadata.ipynb

Explored adding information from a very simple registry file to the default 
[OEMetadata template](https://github.com/OpenEnergyPlatform/oemetadata/blob/develop/oemetadata/latest/template.json). Manually altered information and validated against the schema. 

- Input: friendly_config.yml (inspired by [friendly_data](https://sentinel-energy.github.io/friendly_data/registry.html))
- Output: None. All printed to screen.

## quickie_oemetadata.ipynb

Continued explorations of OEMetadata and registries that eventually became [aedg-metadata](https://github.com/acep-aedg/aedg-metadata/tree/main).

- Inputs:
  - `../config/public/public_communities_monthly_generation.yml`
  - `../registry/fields.yml`
  - `../registry/licenses.yml`
  - `../registry/agents.yml`
- Output: `../metadata/public/public_communities_monthly_generation.json`
