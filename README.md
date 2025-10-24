# 📘 Machine Learning Specialization — Course 1 · Week 3

[![UV](https://img.shields.io/badge/uv-v0.4-blue)](https://github.com/astral-sh/uv) [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/) [![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

Brief, self-contained repository for Week 3 assignment and optional labs. Organized for quick setup and reproducible experiments using UV.

Prerequisites: Python 3.8+, UV package manager, Jupyter Notebook / JupyterLab.

Install UV
- macOS / Linux
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```
- Windows (PowerShell)
```powershell
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```
- pip
```bash
pip install uv
```

Clone and prepare project
```bash
git clone <repository-url>
cd ml-specialization-c1-w3
uv sync
uv run jupyter notebook
```
Open `ml-specialization-c1-w3.ipynb` to start.

Development commands
- install all dependencies
```bash
uv sync
```
- install production only
```bash
uv sync --no-dev
```
- add packages
```bash
uv add numpy pandas matplotlib
```
- add dev packages
```bash
uv add --dev pytest black jupyter
```
- run scripts
```bash
uv run python script.py
uv run python -m module_name
```
- launch Jupyter
```bash
uv run jupyter notebook
uv run jupyter lab
```
- update and inspect dependencies
```bash
uv sync --upgrade
uv tree
```

Key dependencies: numpy, pandas, matplotlib, scikit-learn, scipy, jupyter, ipywidgets, ipympl, notebook, black, pytest, jupyterlab.

Usage
- restart kernel and run all cells after installing dependencies.
- execute notebook cells in order and save frequently.
- enable interactive widgets/plots:
```bash
uv add ipywidgets ipympl
uv run jupyter nbextension enable --py widgetsnbextension
uv run jupyter nbextension enable --py --sys-prefix ipympl
```

Troubleshooting
- kernel not connecting
```bash
uv run python -m ipykernel install --user --name=uv-ml-env
```
then select `uv-ml-env` in Jupyter.

- missing packages
```bash
uv pip list
uv add <package-name>
uv sync
```
- datasets not found: confirm `data/` exists and you are in project root.

Performance tips
```bash
uv sync --frozen
uv sync --compile-bytecode
```

Assignment notes: Week 3 topics: logistic regression, regularization, model evaluation, multi-class classification. Submission: complete all required cells, ensure tests pass, save notebook with outputs, follow course submission rules.

Contributing
```bash
# fork → branch → change → test → pull request
uv run pytest
```

Resources: UV https://github.com/astral-sh/uv, Jupyter https://jupyter.org, Scikit-learn guide https://scikit-learn.org/stable/user_guide.html, Matplotlib tutorials https://matplotlib.org/stable/tutorials/index.html.

License: part of the Machine Learning Specialization — follow course academic integrity policies.

Happy learning — commit regularly and follow good data-science practices.
