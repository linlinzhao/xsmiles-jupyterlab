# XSMILES visualizations in Jupyter Lab

A Custom Jupyter Lab Widget to visualize SMILES-based and atom-based scores.

## Please Cite

If you use XSMILES, the use cases, its code, or the generated explanations, please cite our article:

**Article in preparation**, a preprint should appear mid September!

```
Heberle, H., Zhao, L., Schmidt, S., Wolf, T., & Heinrich, J. (2022). XSMILES: interactive visualization for molecules, SMILES and XAI scores. Article in preparation.
```

```BibTeX
@article{Heberle2022XSMILES,
author = {Heberle, Henry and Zhao, Linlin and Schmidt, Sebastian and Wolf, Thomas and Heinrich, Julian},
doi = {},
journal = {Article in preparation},
month = {},
number = {},
pages = {},
title = {{XSMILES: interactive visualization for molecules, SMILES and XAI scores}},
volume = {},
year = {2022}
}
```

![JupyterLab Notebook](/examples/widget_example.png)

## Availability and examples

- [XSMILES main page](https://github.com/Bayer-Group/xsmiles)

- [Demo website](https://bayer-group.github.io/xsmiles/dist/web/)

- [HOW TO use XSMILES with JupyterLab notebook](examples/xsmiles_examples.ipynb)

- [More examples with JupyterLab](https://github.com/Bayer-Group/xsmiles-use-cases)

- [Unofficial Pypi repository](https://pypi.org/project/xsmiles/)

- [KNIME component? Check the main page](https://github.com/Bayer-Group/xsmiles)

## Example Notebook with a how-to

To use XSMILES with Jupyter Lab you need to install the package with pip **and have internet connection** while using it.

RDKit MinimalLib is downloaded by your browser.

Please check this notebook to see **how to use** the tool: [Notebook](examples/xsmiles_examples.ipynb)

Note that it is only being tested with Jupyter**Lab**. A reason for you to use Lab is the space available for visualizations, which is much better than in regular Jupyter notebooks. We also had problems with the installation for non-Lab notebooks.

## Installation

### Quick example - create conda environment and installs xsmiles

```bash
conda create --name xsmiles_env python=3.7 -c conda-forge # create conda env with python 3.7

conda activate xsmiles_env # activate the created env

# install dependencies for the example notebook
conda install -c conda-forge jupyterlab rdkit matplotlib

# You can install the latest official version from this repo with: 
# pip install xsmiles-0.2.2-py2.py3-none-any.whl
# Unofficial pypi xsmiles:
pip install xsmiles 

jupyter lab examples/xsmiles_examples.ipynb # run a notebook with jupyter lab
```

### Quick example - create environment with python venv
```bash
# tested with python 3.8
python -m venv xsmiles_env
# activate env
source ./xsmiles_env/bin/activate

# You can install the latest official version from this repo with: 
# pip install xsmiles-0.2.2-py2.py3-none-any.whl
# Unofficial pypi xsmiles:
pip install xsmiles

# install dependencies for the example notebook
pip install jupyterlab rdkit matplotlib 

jupyter lab examples/xsmiles_examples.ipynb
```

## Uninstall

- `pip uninstall xsmiles`
- `rm -r <path-to:>/share/jupyter/labextensions/xsmiles`
- `jupyter labextension list`


## Development

Please check the `DEVELOPMENT.md` file.
