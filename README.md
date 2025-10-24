# 📘 Machine Learning Specialization — Course 1 · Week 3

Brief, self-contained repository for the Week 3 assignment and optional labs.

## Overview
This repo contains notebooks, data pointers, and instructions to complete Week 3 graded tasks and optional lab exercises. Organized for quick setup and reproducible experiments.

## Contents
- Week 3 assignment notebook(s) (graded)  
- Optional lab notebook(s) (extra practice)  
- Dependency / environment hints

## Prerequisites
- Python 3.8+
- Jupyter Notebook or JupyterLab
- pip or conda (or uv if the repo uses that manager)

## Quick setup (choose one)

1. Conda (if environment.yml exists)
```bash
conda env create -f environment.yml
conda activate <env-name>
```

2. Virtual environment + pip
```bash
python -m venv .venv
# Activate:
# Linux / macOS:
source .venv/bin/activate
# Windows (cmd):
.venv\Scripts\activate
# Windows (PowerShell):
.venv\Scripts\Activate.ps1

pip install <package1> <package2> ...
```

3. uv project manager (if used)
```bash
uv project init
uv project install
uv project run jupyter
```

If no environment file is present, inspect notebooks for imports and install required packages manually.

## Notebook note
Notebooks primarily contain code cells. Follow in-cell comments and run cells in order; after installing dependencies, restart the kernel and use "Run All".

## Interactive plot recommendations
For interactive matplotlib widgets and ipywidgets:
```bash
pip install ipywidgets ipympl matplotlib notebook
# or with conda:
conda install -c conda-forge ipywidgets ipympl matplotlib notebook
```
Enable notebook extensions (if needed):
```bash
jupyter nbextension enable --py widgetsnbextension
jupyter nbextension enable --py --sys-prefix ipympl
```

## Usage example
Launch a notebook server and open the Week 3 notebook:
```bash
# Activate your environment, then:
jupyter notebook          # or jupyter lab
# Open the appropriate Week 3 .ipynb file in the browser
```

Notes
- Check notebooks for any dataset download instructions or environment-specific steps.
- If you want, a short "How to run the Week 3 assignment" usage walkthrough can be added.
