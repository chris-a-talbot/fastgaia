# *fastgaia*
Designed and implemented by Chris Talbot, based on *gaia* from Grundler et al., [pre-print here](https://www.biorxiv.org/content/10.1101/2024.03.27.586858v2), [GitHub here](https://github.com/blueraleigh/gaia).

*fastgaia* is a Python package implementation of *gaia* that can run up to 30x faster for large tree sequences. *fastgaia* offers a command-line interface and a comprehensive Python function for inferring the geographic locations of ancestors given a tree sequence. After installing, use `fastgaia --help` from terminal or `fastgaia.infer_locations(...)` in your Python console for more details.

**Note**: In simulation tests on a 20x20 plane, *fastgaia* infers coordinates of ancestors within 0.16 units of their correct location across all timescales - this is only 0.01 units worse than *gaia*. *fastgaia* is particularly accurate for very recent ancestors, inferring locations within 0.001 units of the locations inferred using *gaia*. However, it should still be noted that *fastgaia* provides improved efficiency at the expense of accuracy. While inferences for more nodes with more recent samples as descendants will be close in accuracy to inferences from *gaia*, inferences in the deep past will be increasingly inaccurate compared to *gaia* without sufficient temporal sampling. Accuracy of discrete state inference remains untested. 

## Features

- **Continuous Inference**: Infers continuous locations of nodes based on provided sample locations or tree sequence individual location data.
- **Discrete Inference**: Infers discrete states of nodes using a transition cost matrix.
- **Flexible Output**: Outputs results in CSV format for easy analysis.

## Installation

You can install fastgaia via pip:

```bash
pip install fastgaia
