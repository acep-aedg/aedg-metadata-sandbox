# Schema

## From Original

`datapackage_v2.json` is a copy of https://datapackage.org/profiles/2.0/datapackage.json. There used to be another schema called `tabular-data-package` but that was discontinued in version 2.0.

Note: Not sure what is going on with the version, because the document with `2.0` in the URL has this section:

```json
  "properties": {
    "$schema": {
      "default": "https://datapackage.org/profiles/1.0/datapackage.json",
...
```

https://datapackage.org/standard/data-package/#dollar-schema says

> The default value is https://datapackage.org/profiles/1.0/datapackage.json and the recommended value is https://datapackage.org/profiles/2.0/datapackage.json.


### Validation

``` python
from frictionless import validate

report = validate('table.csv', schema='schema.json')
print(report)

# or
package.validate()
```

and

``` shell
frictionless validate capital-invalid.csv
```

## Examples

1. Jesse made a `data-package` for PCE data [metadata.json](https://github.com/acep-uaf/pce-database/blob/main/src/database/data/metadata/metadata.json) which I have renamed `pce_example.json`
2. `rca_electric_certificates_datapackage.json` is a `tabular-data-package` created and validated by uploading a CSV file to the [Data package Creator](https://create.frictionlessdata.io) ([usage instructions](https://okfnlabs.org/blog/2018/02/05/data-package-creator.html)).
  a. Note: https://datapackage.org/overview/changelog/ says `tabluar-data-package` has been removed in favor of `type: "table"`
  b. So don't use the Data Package Creator because it is based on outdated specs.
3. `test_datapackage.json` was made with Python in the Jupyter notebook `make_package.ipynb` as proof of that concept.
