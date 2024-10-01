# fastgaia

fastgaia is an implementation of gaia (Grundler et al., [pre-print here](https://www.biorxiv.org/content/10.1101/2024.03.27.586858v2), [GitHub here](https://github.com/blueraleigh/gaia)) that can run 30x faster for large tree sequences in continuous space and improves inferences in the presence of internal samples.

## Features

- **Continuous Inference**: Infers continuous locations of nodes based on provided sample locations or tree sequence data.
- **Discrete Inference**: Infers discrete states of nodes with optional cost matrix considerations.
- **Flexible Output**: Outputs results in CSV format for easy analysis.

## Installation

You can install fastgaia via pip:

```bash
pip install fastgaia
