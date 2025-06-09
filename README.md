# Metadata Sandbox

Testing methods of creating Frictionless and Open Energy Metadata for the Alaska Energy Data Gateway

This repository uses Jupyter Notebooks to explore creating metadata from a template CSV file and stashing elements in YAML registry files. None of this code is used in production. Each notebook approches the problem in a different way. 

## Set-up

This repository was set-up using the `uv` package manager as a way of exploring that as well.

``` shell
uv init
uv add frictionless
uv venv
uv sync
source .venv/bin/activate
uv add oemetadata
```

## Jupyter Notebooks

In base directory with venv activated:

```shell
uv run --with jupyter jupyter lab
```

Opens in a browser. Got initial code from https://carpentries-incubator.github.io/frictionless-data-agriculture/index.html.

Note: `uvx` will start up Jupyter Lab, but the environment is wrong and it can't find `frictionless`.
