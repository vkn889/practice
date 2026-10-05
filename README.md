# IDP Practice Sandbox

Jupyter sandbox for IDP quiz practice. Python 3.13.5, managed with [uv](https://docs.astral.sh/uv/).

## Setup (once, after cloning)
```bash
uv sync                                   # creates .venv with the exact pinned packages
uv run python -m ipykernel install --user --name idp-practice --display-name "IDP Practice (Python 3.13)"
cp templates/sandbox.ipynb notebooks/     # optional starter notebook
```

## Start
```bash
uv run jupyter lab
```

## Your work stays local
Everything in `notebooks/` and `data/` is git-ignored, so your notebooks and datasets
stay on your machine and you won't receive anyone else's. Only the environment setup
(`pyproject.toml`, `uv.lock`, `.python-version`, `templates/`) is shared.

## Add a package
```bash
uv add <package>
```
