# P4AIDS - EDA Tabular

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run Notebook

```bash
source .venv/bin/activate
python -m ipykernel install --user --name p4aids-eda-tabular --display-name "Python (.venv) P4AIDS EDA"
jupyter lab
```

Then open `tabular_data.ipynb` and select the kernel `Python (.venv) P4AIDS EDA`.

## Fix for `TqdmWarning: IProgress not found`

This project requires `ipywidgets` so `tqdm.auto` can use notebook widgets.
If you still see the warning, restart the Jupyter kernel and re-run all cells.

