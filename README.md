# AEDG Metadata

To create Frictionless metadata for the Alaska Energy Data Gateway

## how I set-up

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
