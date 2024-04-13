# Python-Project-Template

This is a template repository. Please initialize your python project using this template.

1. Make sure you have a right python version installed locally and change the version of python from the files below
   - `.github/workflows/ruff.yml`
   - `pyproject.toml`

2. `project_name` is your project package name including src.

## Installing and Using the Package

You can install the package locally from the top-level directory:
```python
python -m pip install --upgrade pip build
python -m build
python -m pip install .
```

Distribute
If you want others to install your package via pip directly, you can upload it to PyPI. This requires an account on PyPI and then you can upload using Twine:
```
python -m pip install --upgrade twine
twine upload dist/*
```

## Ruff Usage
Here is how you might proceed with checking for issues:
```
ruff check .
```
If you need to fix issues automatically and if ruff supports it, you would typically see an option like `--fix` mentioned in the documentation or help command:
```
ruff check --fix .
```