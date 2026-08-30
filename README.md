<div align="center">
  <img src="assets/orthouniversity_logo.png" width="250">

  # OrthoUniversity
</div>

Interactive demo notebooks for trying out our bioinformatics tools, designed to run in Jupyter Notebook or JupyterLab with minimal setup. Each notebook walks through installing a tool, running it on example data, and exploring the output — no prior experience with the tool required.

## What's inside

| Notebook | Tool | Description |
|---|---|---|
| [`orthofinder_demonstration.ipynb`](orthofinder_demonstration.ipynb) | [OrthoFinder](https://github.com/OrthoFinder/OrthoFinder) | Orthogroup inference, gene trees, species trees, and orthologue analysis on example proteome data |

More tool demonstrations will be added over time — each lives in its own notebook so you can run just the one you're interested in.

## Getting started

### 1. Prerequisites

You'll need Python 3 installed on your machine (Linux is recommended for these demos). Check your version:
```bash
python3 --version
```

### 2. Set up a virtual environment

From a terminal, in the folder where you want to work:
```bash
python3 -m venv .venv
source .venv/bin/activate      # on Windows: .venv\Scripts\activate
```

### 3. Install Jupyter

```bash
pip install jupyterlab
```
(Prefer the classic Notebook interface instead? `pip install notebook` works the same way.)

### 4. Get the notebooks

Clone this repository:
```bash
git clone https://github.com/OrthoFinder/OrthoUniversity.git
cd OrthoUniversity
```

### 5. Launch Jupyter

```bash
jupyter lab
```
or, for the classic Notebook interface:
```bash
jupyter notebook
```
This opens in your browser automatically. From the file browser on the left, open the notebook for the tool you want to try (e.g. `orthofinder_demonstration.ipynb`).

### 6. Run the notebook

Each notebook is self-contained and installs its own tool-specific dependencies in its first few cells — just run the cells in order from top to bottom (`Shift + Enter` runs a cell and moves to the next one), or use **Run → Run All Cells** from the menu.

> **Note:** Some notebooks create their own isolated environment (e.g. a dedicated virtual environment for the tool being demonstrated) as part of their setup cells, separate from the `.venv` running Jupyter itself. This keeps each tool's dependencies from interfering with one another. Follow the instructions inside each notebook — they're written to be run start to finish without extra setup beyond what's described above.

## Running in the cloud

These notebooks are also designed to work in cloud-hosted Jupyter environments (e.g. JupyterHub, Binder). Since each notebook installs its own dependencies in-cell rather than relying on pre-configured local tools, they should run the same way regardless of environment — provided the environment has outbound internet access (for downloading tools and packages) and a Python 3 kernel available.

## Contributing

Have a tool you'd like to see demonstrated here? Open an issue or submit a pull request with a new notebook following the same self-contained setup pattern as the existing ones.

## License

This project is licensed under the terms of the [MIT License](LICENSE).
