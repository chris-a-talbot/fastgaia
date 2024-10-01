# *fastgaia*

*fastgaia* is a Python package implementation of gaia (Grundler et al., [pre-print here](https://www.biorxiv.org/content/10.1101/2024.03.27.586858v2), [GitHub here](https://github.com/blueraleigh/gaia)) that can run up to 30x faster for large tree sequences in continuous space.

*fastgaia* offers a command-line interface and a comprehensive Python function for inferring the geographic locations of ancestors given a tree sequence. After installing, use `fastgaia --help` from terminal or `fastgaia.infer_locations(...)` in your Python console for more details.

## Features

- **Continuous Inference**: Infers continuous locations of nodes based on provided sample locations or tree sequence data.
- **Discrete Inference**: Infers discrete states of nodes with optional cost matrix considerations.
- **Flexible Output**: Outputs results in CSV format for easy analysis.

## Installation

You can install fastgaia via pip:

```bash
pip install fastgaia
