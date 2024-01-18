# Introduction to NLP

This README provides instructions on how to set up and run the Jupyter notebooks for the introduction to NLP (Natural Language Processing) workshop.

It uses Poetry for dependency management. Also, all notebooks can be run in google colab just by clicking in the button in each notebook.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- Python 3.7 or higher
- Poetry for Python dependency management

## Installation

### Step 1: Install Poetry

Poetry is a tool for dependency management and packaging in Python. To install Poetry, run the following command in your terminal:

```bash
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
```

Or, if you are using Windows PowerShell:

```powershell
(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python -
```

After installation, make sure to restart your terminal or run the following to get the `poetry` command available in your current session:

```bash
source $HOME/.poetry/env
```

For more detailed instructions, visit the official Poetry documentation: https://python-poetry.org/docs/#installation

### Step 2: Clone the Project Repository

Clone the project repository to your local machine using the following command:

```bash
git clone <repository-url>
cd <repository-name>
```

Replace `<repository-url>` with the URL of the project's Git repository and `<repository-name>` with the name of the directory where the repository is cloned.

### Step 3: Install Dependencies Using Poetry

Navigate to the project directory where the `pyproject.toml` and `poetry.lock` files are located and run the following command:

```bash
poetry install
```

This will install all the necessary dependencies as specified in the `pyproject.toml` file.

### Step 4: Activate the Poetry Virtual Environment

To activate the virtual environment managed by Poetry, run:

```bash
poetry shell
```

This will spawn a new shell subprocess, which is configured to use the virtual environment.

### Step 5: Launch Jupyter Lab

With the dependencies installed and the virtual environment activated, you can now launch Jupyter Lab to access the notebooks:

```bash
jupyter lab
```

This command will start the Jupyter Lab server and open it in your default web browser. From there, you can navigate to the `notebooks` directory and open any of the `.ipynb` files to begin working on the NLP tasks.

## Working with Notebooks

The `notebooks` directory contains several Jupyter notebooks that you can use to learn and experiment with NLP concepts:

- `01-basic-ml-classification-tabular-data.ipynb`
- `02-basic-sentiment-classification-dictionary.ipynb`
- `03-basic-sentiment-classification-supervised-classification.ipynb`
- `04-basic-sentiment-classification-supervised-classification-embeddings.ipynb`
- `05-transformers-text-classification.ipynb`
- `06-text-clustering-with-embeddings.ipynb`

You can also find notebooks with solutions in the `notebooks/notebooks_w_solutions` directory.

## Additional Resources

- For more information on Poetry, visit the [Poetry documentation](https://python-poetry.org/docs/).
- To learn more about Jupyter Lab, check out the [Jupyter Lab documentation](https://jupyterlab.readthedocs.io/en/stable/).

If you encounter any issues or have questions, please refer to the project's issue tracker or contact the project maintainers.
